# Roll call:
   * Roman Shaposhnik
   * Raj Desai
   * John Mertic
   * Vineet Goel
   * Paul Kent

# Agenda:
   * TSC seat election update ( John )
   * Runtime PMC update ( Raj )
   * Operations PMC update ( Tim )
   * Infrastructure update ( Roman )

# AIs: 
   * Roman and Raj to sync up next week on SoftLayer infrastructure maintenance for 2.0 release.

# Notes:
  * John: Vineet is on a TSC! Congrats! Board will recongnize it at a future meeting (at around november November)

  * Raj: Scott is leaving, transition will be covered at the next meeting.
        Runtime PMC update: Hive has a PR submitted. HCat will be
        included (as per PMC decision). We have to get HCFS done as well,
        but for now lets separate Hive pull request from HCFS work. Matt F
        is working on the first draft of the SPEC for HCFS (ODPI-168).
        An oustanding issue for HCFS is what to do with testing Roman sent
        an email out last week asking for feedback. The idea is to get it and
        then ask RT for guidance on how to proceed. Since Scott is leaving
        PC will be presumed an HCFS driver from now on. Tang Ping will help.
        Question on final SPEC approcal was asked and John clarified that
        final approval is only required at the end of the release. Other than
        that it is whatever PMC feels comfortable with.

  * Roman: Operations PMC has prepared the first real draft and also first cut
        of the reference implementation Ambari artifacts. There's still quite a bit
        of outstanding work (all of it is tracked on JIRA) but we're confident that next
        week we can get the SPEC to a state that Runtime spec is at this week.
        We still not much of a clue as to how this is going to be tested though.

  * Roman: it was assumed that the build and other infrastructure migration will
        happen to LF maintained services in time for 2.0 release. After talking to
        the LF team responsible for shared infrastructure it is clear that there's a
        non-trivial amount of process to be considered compared to a free-for-all
        SoftLayer VMs that IBM is still graciously donating to us. Thus the proposal
        is to keep using SoftLayer for 2.0 and focus on hiring a dedicated RE position
        within the LF team to migrate the infra past 2.0 release. Roman and Raj are
        to sync up next week to make sure that karma to SoftLayer is shared so
        that if anything goes down there's more than one person to fix it.