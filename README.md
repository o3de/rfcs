[O3DE RFCs]: #O3DE-rfcs

Many changes, such as bug fixes and documentation improvements can be
implemented and reviewed via the normal GitHub pull request workflow.

Some changes are "substantial", and we ask that these be put through a
bit of a design process and produce a consensus among the O3DE community and
the SIGs.

The "RFC" (request for comments) process is intended to provide a consistent
and controlled path for new features to be added to O3DE.

## Table of Contents
[Table of Contents]:

  - [When you need to follow this process]
  - [Before creating an RFC]
  - [RFC Process]


## When you need to follow this process
[When you need to follow this process]: #when-you-need-to-follow-this-process
You need to follow this process if you intend to make "substantial" changes to O3DE, or its documentation, or any other projects under the purview of the O3DE Governing board. What constitutes a "substantial" change is evolving based on community norms, but may include the following:

* A new feature that creates new API surface area, and would require a feature flag if introduced.
* The removal of features that already shipped as part of the release channel.
* The introduction of new idiomatic usage or conventions, even if they do not include code changes to O3DE itself.

Some changes do not require an RFC:

* Rephrasing, reorganizing or refactoring (depending on magnitude)
* Addition or removal of warnings
* Additions that strictly improve objective, numerical quality criteria (speedup, better browser support)
* Additions only likely to be noticed by other implementors-of-O3DE, invisible to users-of-O3DE.

Note: If you submit a pull request to implement a new feature without going through the RFC process, it may be closed with a polite request to submit an RFC first.


## Before creating an RFC
[Before creating an RFC]: #before-creating-an-rfc
A hastily-proposed RFC can hurt its chances of acceptance. Low quality proposals, proposals for previously-rejected features, or those that don't fit into the near-term roadmap, may be quickly rejected, which can be demotivating for the unprepared contributor. Laying some groundwork ahead of the RFC can make the process smoother.

Although there is no single way to prepare for submitting an RFC, it is generally a good idea to pursue feedback from other project developers beforehand, to ascertain that the RFC may be desirable; having a consistent impact on the project requires concerted effort toward consensus-building.

The most common preparations for writing and submitting an RFC include talking the idea over in the SIG areas on the O3DE discord, and discussing the topic in O3DE Discussions. You may file issues on this repo for discussion, but these are not actively looked at by the teams.


## The RFC Process
[RFC Process]: #rfc-process

* When there is a significant change to O3DE being proposed an RFC should be created.
* The author fills out an RFC Issue, using a template, in the either, the responsible SIG's RFC Repository (e.g. https://github.com/o3de/sig-presentation/tree/main/rfcs) OR, if they are unsure which SIG should own the RFC, in the O3DE/RFC Repo (https://github.com/o3de/rfcs/issues). RFCs in O3DE/RFC will be triaged regularly during SIG triage.
* Authors should put care into the details: RFCs that do not present convincing motivation, demonstrate understanding of the impact of the design, or are disingenuous about the drawbacks or alternatives tend to be poorly-received.
* RFC issue is submitted by the author. As an issue the RFC will receive design feedback from the larger community, and the author should be prepared to revise it in response.
* The author builds consensus and integrates feedback. RFCs that have broad support are much more likely to make progress than those that don't receive any comments.
* SIG leads triage all RFCs as part of their triage process. Once there is enough feedback the SIG should determine if the RFC is a candidate for inclusion in O3DE.
* RFCs that are candidates for inclusion in O3DE will enter a "final comment period" lasting 3 calendar days. The beginning of this period will be signaled with a comment and tag on the RFCs pull request.
   * An RFC can be modified based upon feedback from the team and community. Significant modifications may trigger a new final comment period.
   * An RFC may be rejected by the team after public discussion has settled and comments have been made summarizing the rationale for rejection. A member of the team should then add the appropriate rejection label and close the RFCs associated issue.
* If SIG leads accept the RFC at the close of its final comment period:
    * The RFC issue will be labeled 'active' and a Pull Request with all the attachments should be created in the SIG's RFC repo, labeled as 'active' and linked to the RFC.
* When it is time to break out the RFC into workable issues, these should be created in O3DE/O3DE and linked back to the RFC Issue.

**O3DE's RFC process owes its inspiration to the [Rust RFC process], and the [Ember RFC process]**

[Rust RFC process]: https://github.com/rust-lang/rfcs
[Ember RFC process]: https://github.com/emberjs/rfcs
