% Replication and Independent Verification
% Laleh Behjat, Bruce Childers, Eric Eide, Grigori Fursin, Yolanda Gil, Simon Harper, Alex K. Jones, Shriram Krishnamurthi, Jimmy Lin, Patrick Madden, Catherine McGeoch, and Michela Taufer.
% 16 October 2015

Beyond research integrity, and their defining factor of the scientific method, replication and independent verification is about leveraging and accelerating our research productivity by having good clear access to what others have done. Third-parties can build from other people's ideas more quickly and easily, we consider this to be a huge accelerator. 

Replication and independent verification of results are commonplace in many scientific fields. These practices help avoid misunderstandings, provide greater confidence in reported results, and enable the detection of both unintentional error and deliberate fraud. By comparison with fields such as physics, chemistry, and medicine, computer science is clearly lagging in this regard; replication of experiments is rare, and activities such as paper correction or retraction are virtually unheard of.

This document corrects this situation by setting out the view of the ACM SGB in relation to replication and independent verification of results. Therefore Special Interest group (SIG) focused views and requirements can be adopted into the central Association of Computing Machinery (ACM) publications process.

### Scope & Overlaps
{>> Joint Statement with ACM Publication Board Digital Library working group on Data, Software, and Reproducibility in publishing (ACM-DSR) to go here. This will set out the areas of responsibility and overlap. <<}

## Introduction

The scientific method is based on empirical data and the replicability of those experiments used to collect this data by third parties. However, in Computer Science the ability to replicate experiments is limited because there are few peer reviewed routes for experimental replication.

Our limited ability to replicate experiments -- due to a lack of public data -- means that are domains do not strictly follow the scientific method, and as such are sometimes seen as less rigorous than other scientific domains. Indeed, we may go further and suggest that:

1. Methodical data collection and experimentation is variable because the data may never been seen by a third party;

1. Experiments to confirm the science are not repeated as the data and experimentation methodology is not available, and without a publication route there is no value in doing so; and

1. Data collection and accurate experimentation is not seen as being important for citation and publication of the data alone, and is seen more as a second class citizen to an system-based technical paper.

Other sciences (Physics, Ecology / Biology, Medicine etc.) recognise the value of their data as it costs (often) enormous amounts of time, effort, and money to acquire. As a discipline we need to plug this gap. In this case, the charge of the task force is to develop proposals on how ACM can bring current replication and verification practices in line with the rest of the scientific community. Specifically, the following questions are of interest.

1. **Experiences**: Across the SIGs, what mechanisms are in place to enable replication and verification efforts? Are they sufficient to catch errors or deliberate fraud (and have they in fact done so?). Can these processes be improved or encouraged in some way?

1. **Expectations**: What are reasonable expectations from creators, with regards to enabling replication and verification? How can these expectations be made compatible with the review process in conferences, symposia, journals? Should there be different expectations during review, and after paper acceptance?

1. **Retractions**: If published work fails to be replicated, appears to contain significant errors, or even appears to be fraudulent -- what mechanisms should be in place to investigate the matter? Who would such concerns be communicated to? Who would perform investigation, and decide the matter? And if errors, deception, or fraud are confirmed — what should the ACM, as a publisher, do? Should there be corrections, annotations noting the errors, paper retraction?

The SIGs, with elected leaders representing the various research communities of computer science, are a logical group to engage in setting policy. The SIG leaders will be familiar with typical practices within their areas of expertise. With control of many of the major publishing venues, this group also has the ability to enact change.

The critical point for widespread adoption of replication is a shared understanding of what this means, what items actually support replication, and what a flexible framework to house these aspects looks like. Flexible is key if we are to accommodate all ACM SIGs, while having enough commonalities to  present a holistic structure.

The key issue here is the replication and support or repudiation of the work based on the claims set out in the accompanying paper (on which the evaluation of the research artefacts are based). Along with the ability to convey this information, and the results produced, at a high level to interested parties who may not be technical specialists within the area.

We are trying to convey surety to other researchers and the public at large that this work is reproducible, or has the potential to be reproducible. And that any discussions surrounding repudiation and retraction are open and transparent including (maybe especially) when there is a suggestion of academic malpractice.

## Experiences
Our initial aim was to collect and understand the experiences of different groups within the ACM SIG structure. This was, so that we could decide what approaches to pursue for the subsequent **expectations** and **retractions** best practice, and which approaches could be implemented for all. However as detailed in the "Scope and Overlap" section the collection of best practice and experiences was already well underway as part of the remit of the ACM-DSR. In this case, we chose to adopt their best practices so as not to repeat work and so that we could move quickly to discussing **expectations**.

This said we did contribute best practice and current work around Artefact Evaluation and the experiences of SIGPLAN and SIGSOFT, and the CGO and PPoPP (2015, 2016) conferences.  This best practice was included in the ACM-DSR documents.

To summarise, the ACM-DSR have collected around 650 pages of best practice experiences. Have summarised these as a 47 page document, and have further condensed this as a 10 page executive summary. The outcomes of this summarisation process can be thought of as follows.

{>> A One Page Summary will be placed here once the final small document is created <<}

## Framework
In this case, we see this work as being a flexible framework which is initially populated with best practice. It is worth stating that post ‘Experiences’ the work on artifact evaluation as described at [Artifact Evaluation](http://www.artifact-eval.org/) (AE) has heavily influenced the work on this framework. This is mainly because the procedure for artifact evaluation is already well used and understood, and forms the thinking behind many of the embryonic tools supporting the area. We expect the AE work to be updated by the ACM-Publications Board and this variant used as a starting point to enable SIGs to populate this framework with their own expectations of what an artifact means within their domain, and what it means to evaluate it.

Currently this draft relies on AE as the ACM-Pubs variant has not yet been created.

## Expectations
When discussing replication we need to understand what are reasonable expectations. Reasonable expectations from creators with regards to enabling replication verification of their paper -- based on the artefacts supplied as accompanying materials to that paper. We must also understand what expectations we have of the review process for conferences, symposia, and journals. Still further, we must also understand what expectations we have of volunteer reviewers and what benefits to a reviewer this enhanced replication process may have (or can be offered).

Realising that a volunteer reviewer is likely to be another academic and that the currency of this academic may be visibility and citation as well as engagement with the community and volunteerism is critical. Finally we need to answer questions as to the different expectations we may have from papers during review and those after paper acceptance.

Therefore, we are interested in detailing what are reasonable expectations. And what are possible inducements for all three stakeholders (the creators, the organisers, and the reviewers). Further describing, how these can be accommodated across the diverse Special Interest Groups which make up the bulk of the membership of the ACM.

The evaluation criteria are ultimately simple. A paper sets up certain expectations of its artifacts based on its content. The evaluators will read the paper and then judge how well the artifact matches these criteria. Thus the evaluators decision will be that the artifact does or does not “conform to the expectations set by the paper”. Ultimately, we expect artifacts to be:
1. consistent with the paper,
1. as complete as possible,
1. documented well, and
1. easy to reuse, facilitating further research.

### Expectations of creators
We are looking to replicate the creator(s) experimental setting exactly so that we can evaluate if the claims detailed in their paper can be replicated and evaluated, or at least if it is possible for the third party to replicate results in the future when, and if, the need arises. It may be that we do not need to evaluate at this time, but that we are concerned that the possibility to evaluate, replicate, repudiate, or confirm the results is available post-hoc.

In this case, and regardless of the artifact submission -- be it software, data,  analysis, etc -- the experimental context must be explicit. This, of course, maybe easier in terms running software than manual mathematical proofs.

To avoid excluding some papers, any artifact that creators wish to submit will accept. As implied above, these can be tools but can also be test suites, models, proofs, data-sets etc. Obviously, the better the artifact is packaged, ie the more explicit the experimental setting is described, the more likely the organisers can work with it.

creators are free to include models, data files, proprietary binaries, etc. in their artifact. We do strongly encourage that they anonymise any data files that you submit.

We recognise that some artifacts may attempt to perform malicious operations by design. These cases should be boldly and explicitly flagged in detail in the readme so review members can take appropriate precautions before installing and running these artifacts.

### Expectations SIGs
SIGs should use the Pubs Board and AE model as a tried and tested starting point. However, each SIG should also have a procedure in place for supporting the particular expectations of that community. Certainly, the expectations of the SIGCHI community may be much different than those in say, SIGPLAN, by which SIGCHI may require American Psychological Association style when discussing a data-set artifact. PRISM statements may be required for systematic reviews for CSUR, CONSORT diagrams for health related -- SIGBio-- computer science.

In all cases, the organisers -- be they ACM journals or ACM SIGs -- should start with ACM-AE and explicitly modify and update to their own needs within that specific community. In this way, full SIG participation is encouraged and no SIG community is excluded.

Further, both the ACM and each constituent SIG should also include a section on expectations, accountability, reproducibility -- a ‘a statement of expectations’ in their code of conduct. This statement is not just words but the SIG will hold the conference accountable to it over time. And must be addressed in the budding process.

In all cases, the organisers (via the SIGs) will accept a video of the artifact in use. These may include screencasts of the software being run on the examples in the paper, traversals of models using modelling tools, stepping through a proof script, etc. The video is, of course, not a substitute for the artifact itself, but this provides an evolutionary path that imposes minimal burden on creators.

### Encouraging Evaluators

Encouraging volunteer evaluators is critical if the process is successful. In this case, academic incentive must be given. This may take the form of:

1. Awards and honours for participating.
1. Naming in the paper acknowledgements.
1. Publication of an accompanying review of the artifact (SIGCHI alt.chi already has a process of publishing review comments against it’s papers).
1. Alt-metric credits via systems like Publions.

However, in all cases experience suggests that student volunteers are the most valuable commodity and are the most likely to see the benefits. The other benefit of using students is to bring them into the scientific process -- remember most of these students have never been  put on a programme committee, especially not at the stage -- so they can be encouraged when they are early in their scientific career. Experience suggests that students are incredibly motivated and excited because they have got something they can put on their resume, they feel like more mature adults in the community. Students can't wait  to get on the committee and they do a phenomenal job in general. If anything they're overly critical.

### Expectations of Evaluators
Evaluators should conform to the instructions set out for them by the ACM-AE/Specific SIG. Support will be provided as AE will be new to most academics. Submission of an artifact does not contain tacit permission to make its content public. Evaluators may not publicise any part of your artifact during or after completing evaluation, nor retain any part of it after evaluation. 

What effort we expect evaluators to expend on an evaluation is difficult to quantify and may be different in each community. However, we would expect the evaluation to take one hour and no more than two hours. If the evaluation including setup is not realisable in this time then the description of the experimental conditions are substandard. In the event that there is a discrepancy between evaluators, those evaluators not able to run the evaluation must document the reasons for its failure. The evaluation committee decides on the the replicability of an artifact. Papers are accepted on condition that if submitted for evaluation they pass.

### Evaluation Order and Invalid Results
Because both the paper and the artifact are reviewed and evaluated, the order these occur in may be problematic. Current best practice is that papers are primary and are reviewed and accepted first, then artifacts are evaluated if submitted. However, this generates a problem whereby an artifact, accompanying an accepted paper, fails evaluation. If this occurs then the decision as to how to proceed is left to the organisers. It maybe that (as current best practice) the paper does not get ‘badged’ as having and evaluated artifact, and no more is said. However, in future it may be that evaluation is compulsory and if an artifact fails evaluation then it's paper is not accepted.
 
## Issues with Artifacts
In some cases , issue with the artifact may come to light; these may be reported in two ways. Those by which the artifact creators find an issue (Self-Reporting) with their artifact, and those which are found by a third-party (Third-Party Reporting). In all case, we initially take an ‘optimistic’ view of the issue by expecting that the problem was created in good faith and that malpractice was not intended. Notification of ratified issues fall into one of four categories: erratum, corrigendum, retraction or addendum, described here.

### Notification
Publishable amendments are represented by a formal printed and online notice in the publication because they affect the publication record and/or the scientific accuracy of published information.

#### Erratum
Notification of an important error made by the ACM publication that affects the publication record or the scientific integrity of the artifact, or the reputation of the creators, or of the journal.

#### Corrigendum
Notification of an important error made by the creator(s) that affects the publication record or the scientific integrity of the artifact, or the reputation of the creators or the publication. All creators must sign corrigenda submitted for publication. In cases where co-creators disagree, the adjudicator will impose the appropriate amendment, noting the dissenting creator(s) in the text of the published version.

#### Retraction
Notification of invalid results. All co-creators must sign a retraction specifying the error and stating briefly how the conclusions are affected. In cases where co-creators disagree,  the adjudicator will impose the appropriate amendment, noting the dissenting creator(s) in the text of the published version.

#### Addendum
Notification of a peer-reviewed addition of information to an artifact, usually in response to third-party requests for clarification. Addenda are published only when the adjudicator decides that the addendum is crucial to the understanding or use of a significant part of the contributed artifact.

### Reporting
We recognise our responsibility to correct errors that we have previously published. Our policy is to consider refutations of artifacts, and to publish them (in concise form) if and only if the reportee provides compelling evidence that a major claim of the original artifact and associated paper was incorrect. It is salient to remember that an artifact does not have to be ‘correct’, it only has to support the claim of the accompanying paper to which it refers, ie artifacts support the claims of a paper, there are no implied claims in and of the artifact itself.

#### Self-Reporting
It may be that an issue with an artifact (whatever that may be) comes to light by the continued experimentation of the creators. Indeed, we would expect that this would be the most likely cause of found issues, as the creating team are most likely to be working consistently on their own artifact. In this case, to encourage self-reporting, we would propose a blame-free mechanism which does not remove the original work, but which replaces it by an updated version, and which details the relevant issues, how they may manifest, and how they may affect the work of others (derivatives). An adjudicator outside the field will be appointed to oversee the case. Self reported issues do not require a retraction. But do require a detailed explanation and a new corrected version, or the current version to be embargoed to prevent further use until a new correct version can replace it.

#### Third-Party Reporting
By actively providing and encouraging artifacts for use, we may also expect third-party investigators to unearth issues with the artifact not previously discovered. Again we provide a blame free reporting method (to encourage dialogue between reporters and artifact creators). The current version is embargoed while a dialogue ensues, overseen by an adjudicator outside the field. This reporting method may also ‘blinded’ so that anonymised  communication flows through the adjudicator in cases where the reporter is concerned that challenging an artifact may have detrimental effects to their career or/and ongoing research. In this case, the adjudicator should senior be enough to not be threatened by any party, and be trusted by both. In this case, mediated discussions continue until consensus. The reporter providing an exact specification of the issues and how it was uncovered, the creator detailing affirming or denying the claim with a detailed accompanying explanation. If found to be correct a new version will update the old and the reports being named co-creators (co-creators) of that version.

### Intent
The creator's intent is difficult to ascertain without a complete investigation. However, some attempt to understand the intent behind an issue should be made.

#### Good Faith Issues
In most cases, we would expect all issues to arise in good faith. Creators did not intended to produce and incorrect artifact, but by the complex nature of work in this discipline, and the artifacts arising from it, issues have arisen. In this case, no action, beyond that detailed above, should be undertaken except  for the correction of the artifact and a posted notification.

#### Incompetence
In some rare cases issues may arise to to incompetence or inexperience. The creators did not intended to produce and incorrect artifact, but due to incompetence or inexperience, issues have arisen. In this case, no action, beyond that detailed above, should be undertaken except for the correction of the artifact and a posted notification.

#### Malpractice
On the very rare occasion that malpractice comes to light in that a creator(s) has knowingly falsified work related to an artifact.  The current version is embargoed while an investigation ensues, overseen by an adjudicator outside the field. This reporting method is ‘blinded’ so that anonymised communication flows through the adjudicator in all cases. In this case, the adjudicator should be senior enough to not be threatened by any party. If proven, the the work should be removed with a statement -- detailing the investigation -- taking its place.

### Derivative Work
If successful we would expect many derivative work to be built upon on an artifact. In this case, those works citing the artifact in question should be notified. An addendum notification added to each derived work detailing any effects of the issue with the derived work, or in the case where the creator(s) of the derived work not replying an addendum detailing this, as a warning to those intending to use the derived work.


## Summary
The ACM code of conduct has not been updated since 1992.  Honesty as one of the criteria, however, a re-write may also consider integrity in the scientific method.


## Afterward
The [ACM](http://www.acm.org) [SGB](http://www.acm.org/sigs/sgb/) Replication Taskforce was initiated at the request of the SGB Chair [Patrick Madden](http://dl.acm.org/author_page.cfm?id=81100092346) in September 2015. SIG Development Advisor [Simon Harper](http://dl.acm.org/author_page.cfm?id=81100139139) was appointed Taskforce Chair to take this forward as well as integrating it into the 'DL-Technology: Data, Software, & Reproducibility' project.

The charge of the task force was to develop proposals on how the ACM can bring current replication and verification practices in line with the rest of the scientific community. Given the range of research topics and problems considered, there was no one-size-fits-all policy. With this in mind this group was open to all voices across the SGB and composed SGB members and other invited experts. The document is also intended to evolve (hence the versioning here, and the versioned releases) and be transparent. By engaging many SIGs in this effort, a degree of consistency was achieved across the ACM.

### Contributors / creators
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
