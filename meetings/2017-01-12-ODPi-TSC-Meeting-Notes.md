# Roll Call
 * Raj Desai
 * Paul Kent
 * John Mertic
 * Alan Gates
 * Roman Shaposhnik

# AIs
 * [Raj] Come back with resolution on fscheck issue
 * [Roman] Get SIGs setup
 * [Roman] Get PMC notified of the approved release scope
 * [Roman] Re-establish the bug scrub meeting on Fri

# Decisions
 * Spark work is pushed to a proposed SIG
 * HBase work is pushed to a proposed SIG

# Discussion

The bulk of our discussion was spent talking about
finalizing ODPi.next release scope. We decided to
to NOT take Spark and HBase work at the PMC level
and instead suggest those areas as potential SIGs.
This is in line with RT recommendation and thus finalizes
ODPi scoping of the ODPi.next release (attached bellow).

It is execution time!

Speaking of which, we also agreed to notify PMCs that
they need to put all appropriate JIRAs into the ODPi
JIRA tracker to describe details of the proposed work.
This is expected to be done in the next two weeks. After
that we're re-instanting our weekly JIRA scrub meetings
on Fri.

TSC also approved the proposed mechanics and scope
of SIGs. Expect SIG announcements shortly.

Finally we talked about fsck tests and HDFS-8809. Raj
is following up to close a loop on that.

# Committed ODPi 2.1 release scope
   0. NOT having any major updates to the composition of
       of ODPi Core (hence release version 2.1).
   1. incremental improvements tracked in the ODPi JIRA:
       https://jira.odpi.org/issues/?filter=10300
   2. Runtime PMC focusing on:
        * improvements to the HCFS portion of the spec
        * improvements to the Hive part of the spec
   3. Operations PMC focusing on:
        * upgrade
        * backwards compatibility
        * validation testsuite for management python scripts
          backward compatibility
        * decoupling HDFS from the stack definitions
   4. expect up to 5 SIGs to produce recommendations
      as part of the ODPi 2.1 release:
         1. Data security/Data Governance [Roman taking a lead]
         2. Streaming and Fast Data analytics [Pradeep taking a lead]
         3. Spark SIG [IBM taking a lead]
         4. HBase SIG [IBM taking a lead]
         5. Performance SIG [Looking for a lead]
   5. Attempt to transition away from having a reference implementation
       by driving upstream Bigtop releases takin its place.