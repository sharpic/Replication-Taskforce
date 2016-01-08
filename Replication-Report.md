% Replication and Independent Verification
% Laleh Behjat, Bruce Childers, Eric Eide, Grigori Fursin, Yolanda Gil, Simon Harper, Alex K. Jones, Shriram Krishnamurthi, Jimmy Lin, Patrick Madden, and Catherine McGeoch.
% 16 October 2015

Replication and independent verification of results are commonplace in many scientific fields. These practices help avoid misunderstandings, provide greater confidence in reported results, and enable the detection of both unintentional error and deliberate fraud. By comparison with fields such as physics, chemistry, and medicine, computer science is clearly lagging in this regard; replication of experiments is rare, and activities such as paper correction or retraction are virtually unheard of.

This document corrects this situation by setting out the view of the ACM SGB in relation to replication and independent verification of results. Therefore SIG focused views and requirements can be adopted into the central ACM publications process.

## Introduction

The scientific method is based on empirical data and the replicability of those experiments used to collect this data by third parties. However, in Computer Science the ability to replicate experiments is limited because there are few peer reviewed routes for experimental replication.

Our limited ability to replicate experiments -- due to a lack of public data -- means that are domains do not strictly follow the scientific method, and as such are sometimes seen as less rigourous than other scientific domains. Indeed, we may go further and suggest that:

1. Methodical data collection and experimentation is variable because the data may never been seen by a third party;

1. Experiments to confirm the science are not repeated as the data and experimentation methodology is not available, and without a publication route there is no value in doing so; and 

1. Data collection and accurate experimentation is not seen as being important for citation and publication of the data alone, and is seen more as a second class citizen to an system-based technical paper.

Other sciences (Physics, Ecology / Biology, Medicine etc.) recognise the value of their data as it costs (often) enormous amounts of time, effort, and money to acquire. As a discipline we need to plug this gap. In this case, the charge of the task force is to develop proposals on how ACM can bring current replication and verification practices in line with the rest of the scientific community. Specifically, the following questions are of interest.

1. Across the SIGs, what mechanisms are in place to enable replication and verification efforts? Are they sufficient to catch errors or deliberate fraud (and have they in fact done so?). Can these processes be improved or encouraged in some way?

1. What are reasonable expectations from authors, with regards to enabling replication and verification? How can these expectations be made compatible with the review process in conferences, symposia, journals? Should there be different expectations during review, and after paper acceptance?

1. If published work fails to be replicated, appears to contain significant errors, or even appears to be fraudulent -- what mechanisms should be in place to investigate the matter? Who would such concerns be communicated to? Who would perform investigation, and decide the matter? And if errors, deception, or fraud are confirmed — what should the ACM, as a publisher, do? Should there be corrections, annotations noting the errors, paper retraction?

The SIGs, with elected leaders representing the various research communities of computer science, are a logical group to engage in setting policy. The SIG leaders will be familiar with typical practices within their areas of expertise. With control of many of the major publishing venues, this group also has the ability to enact change.

# Experiences
{>>START: Cut and Paste this Block<<}
## [Change to your SIG/Organisation]

### Systems Used

### Process Followed

### Changes Made

### Other Comments
{>>END: Cut and Paste this Block<<}

## CGO and PPoPP (2015, 2016)

In 2015 and 2016, CGO and PPoPP decided to adopt the Artifact Evaluation process (described below for SIGPLAN and SIGSOFT) to encourage authors to improve their experimental methodologies and to make their experimental artifacts available to other researchers. We adopted the AE process in its basic form with a small change for a clarification period; i.e., the process used is the same as described on the AE web site (http://www.artifact-eval.org).  The basic process reviews artifacts for accepted papers to ensure the artifacts and experiments are consistent with the results reported in the published paper. Papers that were successfully validated had a validation seal attached to their camera-ready PDF before inclusion in the ACM Digital Library. Upon successful validation, authors are also encouraged to make their artifact and experimental materials publicly available, e.g., using ACM's supplementary material in the Digital Library, although it is not required. 

To form the AE, we invited the program committees of the two conferences to nominate evaluators for the AEC.  The evaluators were a mix of senior PhD students, post doctoral fellows, research scientists, and a few faculty.  In 2016, we added more members to the AEC and invited the past AEC members to also participate, creating a range of experience with artifact evaluation. 

In both years, we made a small change to the basic AE process.  The change was to incorporate a clarification step.  After an initial review, the evaluators were given a means to ask authors to clarify issues with the artifacts. 

In 2016, we made a further change to add sheperding for artifacts.  The AEC, operating through the AE chairs, worked with authors to clarify concerns and fix as many bugs and other issues as possible to get the artifact to the point where it could be successfully validated.  

### Experience


We found the AE process to work quite smoothly for both conferences.  Both conferences are systems oriented; i.e., prototype implementations of compilers, run-time systems, analyzers, debuggers, etc., are used in experiments.  The authors generally packaged these prototypes in virtual machines that could be downloaded and run by the evaluators to replicate experimental results. A few cases, as noted below, required special handling.

During evaluation, bugs were found in the documentation, packaging and scripts to run artifacts.  The clarification step proved important to allow authors to fix smaller concerns and to clarify documentation.   During 2016, the sheperding process permitted authors to fix more complex issues and to clarify how to work with their tools.  Only a few artifacts required sheperding.  In the end, all submitted artifacts were successfully valdiated!  Note the sheperding represents a slight shift in philosophy of AE.  In 2015, the view was to reward authors for doing an exemplary job by awarding the seal.  In 2016, our view changed to treat the process as a "certification" or "validation" step, where the goal is to usher all submitted artifacts successfully through the process.  In this way, we hope the artifacts were improved enough that authors would be more likely to publicly release their materials (when possible).

In both years, a few artifacts required special handling.  These artifacts generally revolved around two issues: 1) the artifacts relied on proprietary and/or commercial tools (where licensing was needed), or 2) the artifacts relied on special hardware access. Our belief is everyone should be encouraged and allowed to participate in AE, regardless of whether they face proprietary issues (i.e., the authors are industrial researchers where their materials cannot be released) or used special machines. To this end, we arranged for authors to provide anonymous remote access to evaluators to get access to the artifacts.  The evaluators were able to use this remote access to replicate experiments.  

In a couple cases, we were unable to resolve the concerns.  In one situation, the industrial researchers could not provide remote access due to company policies.  It may have been possible to sign a nondisclosure agreement for access, but this would have violated anaonymity in reviewing and seemed relatively heavyweight for AE.  In another situation, the authors used a large-scale parallel machine that did not permit anonymous remote access.  Again, this would have violated anonymity of the evaluators and we were unable to accommodate the artifact.  In a third situation, the authors could not provide access to the hardware because it was highly specialized (instrumented for power measurement). Instead, the authors provided access to raw data files from their instrument as a proxy to access to the real hardware for replication.   In a final situation, the authors used a high-end graphics processing card.  For this case, we asked evaluators whether they had the necessary hardware, and we were able to find a couple evaluators with the card.  These evaluators reviewed that artifact.

For evaluation, we felt that being as inclusive and flexible as possible, without sacrificing anonymity or imposing a high burden on evaluators/authors, was critical to achieving a high participation rate.  It is particularly important for industrial researchers. In communities like PPoPP and CGO, there are many industrial researchers and allowing them to participate in AE is critical to the ultimate goal of improving accountability in reserach methods and tools.

Another issue we faced is the definition of "validation".  That is, what are the criteria that reviews should use?    In 2015, authors and evaluators interpreted the term slightly differently in some cases.  For example, some evaluators believed reviewing source code was important for validation, but this was not always made available due to proprietary concerns.  Thus, there were sometimes a mismatch in expectation of the evaluation.  In 2016, we addressed by this by clarifying that "validation" meant "are the artifact materials consistent with the results reported in the paper?".  We left it up to reviewers to interpret and decide how to arrive at the answer to this question.  Generally, evaluators took the packaged mateirals, read the documentation and re-run scripts/experiments to replicate results. Some evaluators tried alternative data sets, alternative setups and so forth. We also provide clarification on several dimensions of criteria, where evaluators evaluated specific aspects and were asked to provide written feedback on certain issues.  We used a standardize form for this purpose.  We also provide authors and evaluators guidelines and steps for evaluation.  These materials are available:

1. http://ctuning.org/ae/submission_extra.html
2. http://cTuning.org/ae/submission.html
3. http://ctuning.org/ae/templates/ae-20151015.tex

### Process vs. Mechanism

During our experience with CGO and PPoPP, it became apparent that it is important to distinguish between process and mechanism. AE is a process by which evaluation can be carried out (with many options).  Equally important is the mechanism used for evaluation.  We found that AE as a process is very smooth and navigates through many thorny issues, e.g., industrial participation and specialized hardware.  It leaves open specific choices, such as evaluation criteria and how closely evaluation outcomes are tied to paper acceptance.  We believe this is the right choice since each community is different.    However, we encountered numerous issues with mechanisms.  As noted above, authors had to worked around several concerns in providing access to their materials.  Additionally, authors all packaged their materials differently, even if they used the same virtual machine (e.g., VirtualBox).  It would greatly help both authors and evaluators to have a set of possible tools available to ease AE, and ultimately, the archiving and distirbution of artifact materials. 


## SIGPLAN and SIGSOFT

SIGPLAN and SIGSOFT have not formally adopted any replication process. In practice, however, numerous conference under the umbrella of these two SIGs (as well as conferences in the same areas but not affiliated with ACM) have informally adopted a fairly uniform process that goes by the name **Artifact Evaluation** (AE). Because this process has been described in detail elsewhere ([AECSite](http://www.artifact-eval.org/), [KVCACM](http://cacm.acm.org/magazines/2015/3/183593-the-real-software-crisis/fulltext)), we provide a brief summary of it here.

The AE process has a few salient highlights:

- The Artifact Evaluation Committee (AEC) is separate from the Program Committee (PC). In pratice, especially by design, there may be a small overlap in members. However, each is constituted by different (cooperating) chairs for different purposes: evaluating papers versus evaluating artifacts.

- The AE process begins only after the PC has made its decisions. This firewall ensures that the AE process can have no impact—in particular, no detrimental impact—on a paper's decision. This was initially put in place to encourage artifact submission, but has largely come to be seen as a positive design decision by the community. As a result, a paper may be accepted but may fail to pass muster with the AEC. What happens when a paper's artifact is found by the AEC to be in egregious violation has intentionally been left unspecified; it is left to the PC chair and the authors to arrive at a reasonable decision.

- The AE process results in a badge that authors can put on papers that pass muster. For this reason, the AEC must make its decisions at least a few days before the camera-ready deadline.

- The AEC is predominantly staffed by junior members of the community (mostly graduate students). There are many reasons for this, as described in the longer articles. The two most important are: (a) they are often the ones most familiar with the tools used for artifacts, and (b) it helps shape the value system of future community leaders.

- The AE process does not dictate what can constitute an “artifact”. More often than not, especially in SIGPLAN and SIGSOFT conferences, these will be software tools. However, they could also be data sets, formal models, proofs, architecture diagrams, and so on. The term “artifact” was specifically chosen to be agnostic to the nature of the artifact.

- The most important detail of the AEC process is the evaluation criterion. The AEC does not evaluate the submitted artifact in isolation. Rather, it evaluates the artifact *relative to the expectations set in the paper* (to do which, the AEC is given a copy of the accepted paper). The paper was presumably accepted based on whatever expectations it set, so AEC members merely check that the provided artifacts satisfy those expectations rather than judging it by (presumed) absolute standards. While this does mean a paper with a “weak” artifact can get a stamp of approval, this is not problematic so long as readers remember the evaluation criterion.

### Systems Used

The AE process does not mandate any particular systems. Indeed, systems are intentionally left unspecified to accommodate a wide variety of possible artifacts. In practice, as of this writing (2016), virtual machine images have become increasingly popular ways of bundling software that can be run relatively painlessly.

### Process Followed

The AEC Chairs convene an AEC independent of and parallel to the PC. The Chairs typically seek out senior graduate students and post-docs: people who have had experience with publication and who have produced some artifacts of note themselves. Submissions to the AEC occur roughly a week after paper acceptance.

An AEC is structured rather like a PC, with two to three reviewers reviewing each artifact, writing detailed comments, and discussing their views. There may even be a brief rebuttal stage, but this depends on the amount of time available between paper decisions and camera-ready.

AECs have found it very productive to undergo a “kick the tires” round, which corresponds roughly to making sure the submitted artifact can be unpacked and, at a rudimentary level, “run” (e.g., the virtual machine login works and the program can be started; the Makefile successfully builds; etc.). The purpose of this round is not to be punitive: failures do not result in automatic rejection. Rather, this catches minor errors (e.g., missing virtual machine password; hidden filesystem dependency); authors are given a chance to submit a revised artifact.

### Changes Made

Not applicable.

### Other Comments

None.


## Afterward
The [ACM](http://www.acm.org) [SGB](http://www.acm.org/sigs/sgb/) Replication Taskforce was initiated at the request of the SGB Chair [Patrick Madden](http://dl.acm.org/author_page.cfm?id=81100092346) in September 2015. SIG Development Advisor [Simon Harper](http://dl.acm.org/author_page.cfm?id=81100139139) was appointed Taskforce Chair to take this forward as well as integrating it into the 'DL-Technology: Data, Software, & Reproducibility' project.

The charge of the task force was to develop proposals on how the ACM can bring current replication and verification practices in line with the rest of the scientific community. Given the range of research topics and problems considered, there was no one-size-fits-all policy. With this in mind this group was open to all voices across the SGB and composed SGB members and other invited experts. The document is also intended to evolve (hence the versioning here, and the versioned releases) and be transparent. By engaging many SIGs in this effort, a degree of consistency was achieved across the ACM.

### Contributors / Authors
- Behjat, Laleh
- Childers, Bruce
- Eide, Eric (SIGOPS)
- Fursin, Grigori
- Gil, Yolanda (SIGAI)
- Harper, Simon (Taskforce Chair)
- Jones, Alex K.
- Krishnamurthi, Shriram (SIGPLAN)
- Lin, Jimmy (SIGIR)
- Madden, Patrick (SGB Chair)
- McGeoch, Catherine

### Colophon
This document is created in standard '[Markdown](http://daringfireball.net/projects/markdown/)' with [pandoc](http://pandoc.org/) [citation additions](http://pandoc.org/README.html#citations). [Critic Markup](http://criticmarkup.com/) is used for [comments](http://criticmarkup.com/users-guide.php). The output format is as yet unknown and so a basic markdown document which can be easily converted to many formats (via pandoc or mmd) is most appropriate. Further, version control via Git is easier using basic text formats.  
