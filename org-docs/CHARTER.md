# Charter for the *NiPreps Community* Organization

This is the organizational charter for the *NiPreps Community* Organization (the "Organization"). By adding their name to the `STEERING-COMMITTEE.md` file, the members of the NiPreps Steering Committee (in the following, *NSC*) agree as follows.

## 1. Mission

The current neuroimaging workflow has matured into a large chain of processing and analysis steps involving a large number of experts, across imaging modalities and applications.
The development and fast adoption of [*fMRIPrep*](https://fmriprep.org) revealed that neuroscientists need tools that simplify their research workflow, provide visual reports and checkpoints, and engender trust in the tool itself.
The NiPreps framework extends fMRIPrep's approach and principles to new imaging modalities.
The mission of NiPreps is to provide end-users (i.e., researchers) with applications that allow them to perform quality control smoothly and to prepare their data for modeling and statistical analysis.
In brief,

> *NiPreps **augment the scanner** to produce data **directly consumable** by analyses*.

We refer to *data directly consumable by analyses* as "*analysis-grade* data" by analogy with the concept of "*sushi-grade (or sashimi-grade) fish*" in that both are products that have been:

* **minimally preprocessed**, but are
* **safe to *consume*** directly.

## 2. NiPreps Steering Committee (NSC)

**2.1 Purpose**. The NSC will be responsible for all technical oversight, project approval and oversight, policy oversight, and trademark management for the Organization.
The NSC is in responsible for organizing and properly promote participation in community meetings called *NiPreps Roundups*.
The frequency, date, time and platform of these *Roundups* are determined by the NSC, but shall occur at least once a calendar year.
Finally, the NSC is also ultimately responsible for securing the coordination of the *NiPreps Technical Monitoring meetings* described in the `PROJECT-CHARTER.md` document.

**2.2 Composition**. The NSC voting members are listed in the `STEERING-COMMITTEE.md` file in the repository.
Voting members may be added or removed by no less than three-quarters (3/4) affirmative vote of the NSC.
The number of members of the NSC is must be an odd number, and it is three (3) as of the approval of this document.
Although not mandatory, members of the NSC preferably are active MAINTAINERS of at least one NiPreps project of those listed in the `PREPS-END-USER.md` file (see section 8 below), be listed as a maintainer of the *TemplateFlow* sibling-organization, or have served in the past.
In particular, this rule must be respected when adding and removing members.
Therefore, the time lapse with an even number of members after the removal of a member should be minimized by appointing a replacement as fast as possible (or even before the removal).
Likewise, when growing the NSC number of members, it must be done by steps of two (e.g., from three to five), and this decision will also require a 3/4 majority.
The NSC will appoint a Chair responsible for organizing NSC activity.
The NSC Chair will be also responsible for the secure management of secrets, access, and permissions to foundational resources such as:
  * GitHub organizations (nipreps and siblings),
  * the [`nipreps-bot`](https://github.com/nipreps-bot) GitHub robot-user,
  * the <nipreps@gmail.org> e-mail account and all associated Google services (e.g., Google Drive),
  * the [`niprepsbot` DockerHub user](https://hub.docker.com/u/niprepsbot) and the [`nipreps` DockerHub organization](https://hub.docker.com/u/nipreps),
  * the CircleCI subscription,
  * the Sentry.io subscription,
  * the [nipreps user at Pypi](https://pypi.org/user/nipreps/),
  * the [NiPreps GH Bot at OSF.io](https://osf.io/2yrct/),
  * the [`nipreps-admin` user at g-node](https://gin.g-node.org/nipreps-admin), and
  * any other service not listed here.

## 3. Voting

**3.1. Decision Making**. The NSC will strive for all decisions to be made by consensus. While explicit agreement of the entire NSC is preferred, it is not required for consensus. Rather, the NSC will determine consensus based on their good faith consideration of a number of factors, including the dominant view of the NSC and nature of support and objections. The NSC will document evidence of consensus in accordance with these requirements. If consensus cannot be reached, the NSC will make the decision by a vote.

**3.2. Voting**. The NSC Chair will call a vote with reasonable notice to the NSC, setting out a discussion period and a separate voting period. Any discussion may be conducted in person or electronically by text, voice, or video. The discussion will be posted under the ["Issues" tab of the `nipreps/GOVERNANCE` repository](https://github.com/nipreps/GOVERNANCE/issues) (that is, this repository) and open to the public. In any vote, each voting representative will have one vote. Decisions by vote require a simple majority vote of all voting members except if specifically noted elsewhere in this Charter (e.g., changes to composition). In simple-majority votes, the Chair of the NSC holds tie-breaking vote.

## 4. Termination of Membership

In addition to the method set out in section 2.2, the membership of a NSC member will terminate if any of the following occur:

**4.1 Resignation**. Written notice of resignation to the NSC.

**4.2 Unreachable Member**. If a member is unresponsive at its listed handle for more than three months the NSC may vote to remove the member.

## 5. Trademarks

Any names, trademarks, service marks, logos, mascots, or similar indicators of source or origin and the goodwill associated with them arising out of the Organization's activities or Organization projects' activities (the "Marks"), are controlled by the Organization. NSC members may only use the Marks in accordance with the Organization's trademark policy. If a NSC member is terminated or removed from the NSC, any rights the NSC member may have in the Marks revert to the Organization.

## 6. Antitrust Policy

The NSC is bound by the Organization's antitrust policy.

## 7. No Confidentiality

Information disclosed in connection with any of the Organization's activities, including but not limited to meetings, Contributions, and submissions, is not confidential, regardless of any markings or statements to the contrary.

## 8. Project Criteria

In order to be eligible to be an Organization project, a project must:

* Be approved by the NSC.
* Agree to follow the guidance and direction of the NSC.
* Use only the following outbound licenses or agreements unless otherwise approved:
  - For code and data as described in the *NiPreps Community* [licensing documentation](https://www.nipreps.org/community/licensing/)
  - For specifications, a community developed and maintained specification agreement, such as the [Open Web Foundation Agreements](http://www.openwebfoundation.org/legal) or [Community Specification Agreement](https://github.com/CommunitySpecification/1.0).
* Have set up a continuous integration and delivery (CI&CD) system, and have an automated release process that includes registration of new version tags onto Zenodo.
* Include and adhere to the Organization's policies, including the trademark policy, the antitrust-policy, and the code of conduct.

In addition to these general criteria, further requirements are set out depending on the project type.

Once a Project has been accepted as part of the Organization, the main fork of said Project must be transferred under [the *NiPreps Organization*](https://github.com/nipreps/)

#### 8.1. End-user applications

These are the actual “*-Preps*”, such as *fMRIPrep*, *dMRIPrep*, *ASLPrep*, or *PETPrep*, as well as their generalizations across populations/species (e.g., *fMRIPrep-rodents*, *fMRIPrep-infants*).
Beyond the general requirements for any project, end-user application must:

* Only and fully support BIDS and BIDS-Derivatives for the input and output data.
* Be packaged as a fully-compliant BIDS-Apps, not just in the user interface, but also in the continuous integration, testing, and delivery.
* Be strictly scoped within preprocessing tasks (i.e., no analysis or irrecoverable preprocessing steps).
* Be agnostic to subsequent analysis, i.e., any software supporting BIDS-Derivatives for its inputs should be capable to analyze data preprocessed with them.
* Be thoroughly and transparently documented (including the generation of individual, visual reports with a consistent format that serve as scaffolds for understanding the underpinnings and design decisions).
* Abide by the *NiPreps Community* charters about scientific authorship and publication.
* Be modular, reliant on NiPreps' *core components* and widely-used tools such as AFNI, ANTs, FreeSurfer, FSL, NiLearn , or DIPY and be extensible via plug-ins.
  Internal sub-modules of end-user applications with potential for generalizing over other “*-Preps*”, should be outsourced as an independent *core component* of the framework.

An updated list of end-user applications is maintained in the document `PREPS-END-USER.md`.

#### 8.2. Core-components: middleware utilities and software infrastructure

These are helper tools covering generalizable tasks of processing, for example, *SDCFlows* for susceptibility distortion estimation and correction which caters to *fMRIPrep*, *dMRIPrep* and *ASLPrep*.

Core-components of *NiPreps* must:

* Have their API (application programming interface) clearly and comprehensively documented.
* Adhere to the *NiPreps* guidelines on versioning and release roadmap.

The maintainers of core-components are recommended to abide by the dispositions of this `CHARTER.md` document and the project-level documents under the `project-docs/` of this `GOVERNANCE` repository.
In the case that a core-component does strictly follow these guidelines and prescriptions, for instance, the repo does not have a `.maint/MAINTAINERS.md` file, then discussions and resolutions rely on the members of the *NiPreps Technical Monitoring meetings*, the maintainers of end-user applications, and, ultimately, the NSC.

An updated list of core-components is maintained in the document `PREPS-CORE.md`.

#### 8.3. Other components: documentation and organizational infrastructure

Repositories and projects supporting the online documentation that are detached from specific end-user applications or core components are listed in the document `PREPS-DOCUMENTATION.md`.

Repositories and projects supporting organizational-level infrastructure are listed in the document `PREPS-INFRASTRUCTURE.md`.

#### 8.4. Sibling organizations

When projects are particularly large, or based on other technical needs, they may be hosted by sister organizations.
An updated list of sibling organizations is maintained in the document `SIBLING-ORGS.md`.

Sister organizations belong to the project category, and therefore decisions are made by consensus of all the maintainers.
The maintainers of the project will be listed on a `MAINTAINERS.md` file hosted under a `GOVERNANCE` repository under the organization.
The *NiPreps* TSC oversees sister organizations in the same ways it oversees projects.

#### 8.5. Upstreaming core components

The experience of *fMRIPrep* demonstrates that it is common to encounter processing steps patterns that replicate across modalities, tasks, or objects of interest.
For example, *sMRIPrep* was identified as a set of workflows that would be useful when used separately or in coordination with other modalities (e.g., DWI), although all the code was originally under the *fMRIPrep*'s repository and was not distributed as a standalone application.
More recently, *SDCFlows* is another example of the same process to minimize redundancies across tools.

When a functionality or feature is identified as of interest to third-parties or other NiPreps components, the Maintainers must be informed about proposals (oftentimes, these proposals will emerge from one or more Maintainers).
Then, the target Project in which the code is going to be upstreamed must be identified:

* **(i) Upstreaming to existing components**.
When the target Project already exists in NiPreps, the Maintainers of the source project and the Maintainers of the target project must be in agreement that the proposal is adequate, and will be together responsible for overseeing the upstreaming process and for ensuring the process is finalized.
The Maintainers of both source and target Projects will operate as if they were a unique maintainers team. Therefore decisions will be consensus-based, with the possibility of initiating appeal processing to the NSC.
* **(ii) Upstreaming to a new project or to a new project under a sibling organization**.
The Maintainers of the source project will proceed with the proposal of a new Organization project following the above guidelines.
An example of this option will be set out by the extraction of the visual report system from *NiWorkflows* as a standalone project called *NiReports*.

In either case, the Maintainers of the source project are responsible for taking all the reasonable measures to preserve the VCS (version control system) history whenever possible, as well as ensuring the `CONTRIBUTORS.md` files of source and target projects are up-to-date and properly represent contributors.
If a contributor is to be transferred (or duplicated) into a sibling organization, they must be properly noticed.

#### 8.6. Upstreaming to other organizations

The most common case for these source code transfers will be the upstreaming of features to NiPype.
As for **8.5.ii**, the Maintainers of the source project are responsible for ensuring that the procedure is carried out correctly:

* keeping track of contributions and crediting thereof;
* communicating with the Maintainers of the receiving Project and coordinating any necessary actions;
* informing affected contributors, explicitly notifying of licensing terms changes, and aborting the upstreaming process if they do not agree with the transfer of their contributions;
* whenever possible, guide and help contributors in the process of upstreaming the code themselves;
* notify the NSC of the outbound code sharing action and assume any decision on the contrary, should it be issued.

## 9. GOVERNANCE changes

Changes to the GOVERNANCE repository can be proposed with the pull-request utility of GitHub.
The NSC will designate one or more [*GitHub CODEOWNERS*](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-code-owners), who will ensure all pull-requests are properly handled, given the opportunity to be discussed and finally approved and merged.
CODEOWNERS will elevate pull-request conversations for consideration by the NSC whenever it is necessary.
The NSC will define how many CODEOWNERS must sign off a pull-request before it is accepted.
In case that a CODEOWNER disagrees with the acceptance decision of a pull-request, the NSC can decide the removal of the individual as a CODEOWNER and replace them if necessary.

## 10. Authorship and scientific publications

All end-user applications and core components have a `.main/` folder directly under the repository's root containing files and scripts to prepare author's lists before publication in scientific journals and or posting preprints or Zenodo entries.
How these resources under `.maint/` must be used is described in the `project-docs/GOVERNANCE.md` document.

End-user applications and core components that make use of other core components of the framework must include "*The NiPreps Developers*" collective of authors listed as a consortium.
All authors within the consortium must be listed in the paper, following the guidelines of the journal to the effect.
The collective of authors list is maintained in the `org-docs/COLLECTIVE-OF-AUTHORS.md` file.

## 11. Ombuds team

The NiPreps Community recognizes the importance of providing a safe and inclusive environment for all community members. To this end, the community has established an *Ombuds team* to serve as a neutral and confidential resource for community members who have concerns or complaints related to the community or its members. The Ombuds team role and responsibilities, as well as the guidelines of its functioning are further described in the file `OMBUDS.md`.

**Enforcement of the Code of Conduct.** Instances of abusive, harassing, or otherwise unacceptable behavior may be reported by contacting an ombudsperson listed in the file `OMBUDS.md`.

## 12. Amendments

Amendments to this charter, the antitrust policy, the trademark policy, or the code of conduct may only be made with at least a 3/4 affirmative vote of the NSC.

---
Part of MVG-0.1-beta.
Made with love by GitHub. Licensed under the [CC-BY 4.0 License](https://creativecommons.org/licenses/by-sa/4.0/).
