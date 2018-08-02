# Roll call:
  * Paul Kent
  * Roman Shaposhnik
  * Alan Gates
  * John Mertic
  * Ganesh Raju
  * Raj Desai

# Agenda:
 1. Chicago Cubs vs Cleveland Indians
 2. Discuss removal of distribution tests from operations spec and focus on ISV conformance instead. (Alan)
 3. Discuss status of HCFS in runtime spec (Roman)
 4. Status report from operations (Roman)
 5. Status report from runtime (Raj)
 6. Status summary on bug count and making the release (Roman)


AI:
  * (Tim) Operations PMC draft detailed answers to what happens beyond ODPi 2.0 release when it comes to having Operation testsuite.
  * (Roman) close the loop with env. changes proposed in addition to HCFS changes.

# Notes

The proposal to go ahead with operations spec not having tests for
the platform vendors but instead of focusing on ISV conformance was
discusses and everybody agreed that it was the way to go for ODPi 2.0
release. The main reason being that since there's very little variations
between vendors shipping Ambari from 2.4 branch stating as much in
our spec should be sufficient way to ensure compatibility.
Two issues were brought up: what happens when Ambari 2.5
comes out and what happens if a hypotherical product "Kambari" wants
to certify. We need Operations PMC to draft detailed answers to these
questions, but it doesn't really affect ODPi 2.0 release. Directionally,
we agreed that we should focus on pushing the backwards compatibility
in the upstream Apache Ambari community and potentially focus on
ISV feedback to shape the overall strategy of testsuite creation. Finally
we agreed that everybody should take one final look at:
   https://github.com/odpi/self-certification-reports/pull/22
before it gets merged.

HCFS work is done. One last look at the proposed changes would be
useful but there are no outstanding work left aside from related changes
to the environment variables.

We discussed the unfortunate situation with Ambari 2.4.0 and 2.4.1
being broken for adding additional component to the cluster. The code
in 2.4 branch seems to fix the problem but that code hasn't been released
yet as 2.4.2. We discussed two potential solutions for ODPi: slip reference
implementation  by a week or put a large # of patches on top of released
version of 2.4.1. In the end we agreed to slip by a week.

Runtime work around adding Hive is mostly done. The only oustanding
testing work is coming from Alan (HCat tests) and he feels comfortable
finishing it on time.

Overall status of the ODPi 2.0 release is goo. We're down to 23 open JIRAs
but quite a few of those are in the pipeline.