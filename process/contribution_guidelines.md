# Contribution Guidelines for ODPi hosted projects

This document captures the general guidelines for contributing to open source projects hosted by ODPi. These guidelines express the provisions in the [ODPi Intellectual Property Policy](https://www.odpi.org/wp-content/uploads/sites/9/2016/09/ODPi_IP_Policy.pdf).

Note that each hosted project may adopt thier own guidelines, which would supercede these provisions in the case of conflict.

## License specification

All source code must clearly identify the open source license used. Refer to the [ODPi Intellectual Property Policy](https://www.odpi.org/wp-content/uploads/sites/9/2016/09/ODPi_IP_Policy.pdf) for the licenses the project supports without having a specific Board of Director waiver.

Requirements to ensure license compliance

- Each repository must contain a license file. Include the plain-text version of the license as a LICENSE file in the top-level directory of the repostiory.
- All source files need to include a header to clearly show the license. ODPi has standardized on including [SPDX short-form license identifiers](https://spdx.org/ids) and a general copyright statement as shown below ( this example is for Apache 2.0 licensed code ):

````
/**
  Copyright Contributors to the [NAME OF PROJECT] Project.

  SPDX-License-Identifier: Apache-2.0
**/
````

For property or configuration files that do not support comments, the license may be omitted. If comments are supported the license header should be included.

Contributors may choose to include a copyright statement specifying themselves and/or their employer (as applicable) as the copyright holder of their contributions, but the ODPi does not require or recommend this.

Finally, please note that pre-existing third-party license notices and copyright notices *should not be modified or removed* by anyone other than the copyright holder. Any questions on including code under a different license than the project should be discussed with the project lead and ODPi Board of Directors.

## Developer Certificate of Origin

We have tried to make it as easy as possible to make contributions. This applies to how we handle the legal aspects of contribution. We use the same approach — [the Developer’s Certificate of Origin 1.1 (DCO)](https://github.com/hyperledger/fabric/blob/master/docs/source/DCO1.1.txt) — that the [Linux® Kernel community](http://elinux.org/Developer_Certificate_Of_Origin) uses to manage code contributions.

We simply ask that when submitting a patch for review, the developer must include a sign-off statement in the commit message.

Here is an example Signed-off-by line, which indicates that the submitter accepts the DCO:

<code>Signed-off-by: John Doe <john.doe@hisdomain.com></code>

You can include this automatically when you commit a change to your local git repository using <code>git commit -s</code>.

### Signoff for commits where the DCO signoff was missed

When bringing in a code repository for the first time, or commits done before the DCO checks are enabled, there would be a series of commits that don't include the sign-off statement. You can retroactively signoff commits you've made by make a commit with your DCO signoff that contains a new text file ( suggested name is past_commits.txt ) with the following contents:

````
The following commits were made pursuant to the Developer Certificate of Origin, even though a Signed-off-by: was not included in the commit message.

<COMMIT HASH> <COMMIT MSG>
...
````

Each user who has made the past commits should have thier own <code>Signed-off-by:</code> line in the commit message.
