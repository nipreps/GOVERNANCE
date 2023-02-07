# Charter for the *NiPreps Community* Organization

This is the organizational charter for the *NiPreps Community* Organization (the "Organization"). By adding their name to the `STEERING-COMMITTEE.md` file, Steering Committee members agree as follows.

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

## 2. Steering Committee

**2.1 Purpose**. The Steering Committee will be responsible for all technical oversight, project approval and oversight, policy oversight, and trademark management for the Organization.
The Steering Committee is in responsible for organizing and properly promote participation in community meetings called *NiPreps Roundups*.
The frequency, date, time and platform of these *Roundups* is determined by the Steering Committee, but shall occur at least once a calendar year.

**2.2 Composition**. The Steering Committee voting members are listed in the `STEERING-COMMITTEE.md` file in the repository.
Voting members may be added or removed by no less than 3/4 affirmative vote of the Steering Committee.
The Steering Committee will appoint a Chair responsible for organizing Steering Committee activity.

## 3. Voting

**3.1. Decision Making**. The Steering Committee will strive for all decisions to be made by consensus. While explicit agreement of the entire Steering Committee is preferred, it is not required for consensus. Rather, the Steering Committee will determine consensus based on their good faith consideration of a number of factors, including the dominant view of the Steering Committee and nature of support and objections. The Steering Committee will document evidence of consensus in accordance with these requirements. If consensus cannot be reached, the Steering Committee will make the decision by a vote.

**3.2. Voting**. The Steering Committee Chair will call a vote with reasonable notice to the Steering Committee, setting out a discussion period and a separate voting period. Any discussion may be conducted in person or electronically by text, voice, or video. The discussion will be posted under the NiPreps category and open to the public, at the [*NiPy Discourse Forum*](https://nipy.discourse.group). In any vote, each voting representative will have one vote. Except as specifically noted elsewhere in this Charter, decisions by vote require a simple majority vote of all voting members.

## 4. Termination of Membership

In addition to the method set out in section 2.2, the membership of a Steering Committee member will terminate if any of the following occur:

**4.1 Resignation**. Written notice of resignation to the Steering Committee.

**4.2 Unreachable Member**. If a member is unresponsive at its listed handle for more than three months the Steering Committee may vote to remove the member.

## 5. Trademarks

Any names, trademarks, service marks, logos, mascots, or similar indicators of source or origin and the goodwill associated with them arising out of the Organization's activities or Organization projects' activities (the "Marks"), are controlled by the Organization. Steering Committee members may only use the Marks in accordance with the Organization's trademark policy. If a Steering Committee member is terminated or removed from the Steering Committee, any rights the Steering Committee member may have in the Marks revert to the Organization.

## 6. Antitrust Policy

The Steering Committee is bound by the Organization's antitrust policy.

## 7. No Confidentiality

Information disclosed in connection with any of the Organization's activities, including but not limited to meetings, Contributions, and submissions, is not confidential, regardless of any markings or statements to the contrary.

## 8. Project Criteria

In order to be eligible to be an Organization project, a project must:

* Be approved by the Steering Committee.
* Agree to follow the guidance and direction of the Steering Committee.
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

At the time of passing these governance documents, the list of current end-user applications of the Organization is:

* [*fMRIPrep*](https://github.com/nipreps/fmriprep)
* [*dMRIPrep*](https://github.com/nipreps/dmriprep)
* [*sMRIPrep*](https://github.com/nipreps/smriprep)
* [*fMRIPrep-rodents*](https://github.com/nipreps/nirodents) -- currently called *NiRodents*
* [*fMRIPrep-infants*](https://github.com/nipreps/nibabies) -- currently called *NiBabies*
* [*MRIQC*](https://github.com/poldracklab/mriqc) -- currently under the PoldrackLab organization and awaiting for transferring over NiPreps.
* *PETPrep* -- currently under a personal repository and awaiting for transfer over to NiPreps.
* [*ASLPrep*](https://github.com/PennLINC/aslprep) -- currently under the PennLINC organization and awaiting for final terms of inclusion and potentially transference over to NiPreps.

#### 8.2. Core-components: middleware utilities and software infrastructure

These are helper tools covering generalizable tasks of processing, for example, *SDCFlows* for susceptibility distortion estimation and correction which caters to *fMRIPrep*, *dMRIPrep* and *ASLPrep*.

Core-components of *NiPreps* must:

* Have their API (application programming interface) clearly and comprehensively documented.
* Adhere to the *NiPreps* guidelines on versioning and release roadmap.

The list of core-components at the time of voting these initial governance documents cover:

* [*SDCFlows*](https://github.com/nipreps/sdcflows)
* [*NiWorkflows*](https://github.com/nipreps/niworkflows)
* [*NiReports*](https://github.com/nipreps/nireports) -- planned in the roadmap
* [*CrowdMRI*](https://github.com/poldracklab/mriqcwebapi) -- awaiting transfer from the PoldrackLab organization and currently named *MRIQC-WebAPI*.
* *MRIQCnets* -- a very vague name to designate several projects investigating DL for QC tasks (e.g., an MRIQC implementation with CNNs or the [MRI face detector](https://github.com/poldracklab/mrideface)).
  These projects are generally undefined, awaiting transfer to the NiPreps organization and open to include new maintainers.

#### 8.3. Sibling organizations

When projects are particularly large, or based on other technical needs, they may be hosted by sister organizations.
An updated list of sibling organizations is maintained in the document `SIBLING-ORGS.md`.
At the moment of writing this charter only two organizations are considered siblings:

* [*TemplateFlow*](https://templateflow.org) ([repo](https://github.com/templateflow/)).
* [*NiPreps-Data*](https://github.com/nipreps-data/)

Sister organizations belong to the project category, and therefore decisions are made by consensus of all the maintainers.
The maintainers of the project will be listed on a `MAINTAINERS.md` file hosted under a `GOVERNANCE` repository under the organization.
The *NiPreps* TSC oversees sister organizations in the same ways it oversees projects.

#### 8.4. Upstreaming core components

The experience of *fMRIPrep* demonstrates that it is common to encounter processing steps patterns that replicate across modalities, tasks, or objects of interest.
For example, *sMRIPrep* was identified as a set of workflows that would be useful when used separately or in coordination with other modalities (e.g., DWI), although all the code was originally under the *fMRIPrep*'s repository and was not distributed as a standalone application.
More recently, *SDCFlows* is another example of the same process to minimize redundancies across tools.

When a functionality or feature is identified as of interest to third-parties or other NiPreps components, the Maintainers must be informed about proposals (oftentimes, these proposals will emerge from one or more Maintainers).
Then, the target Project in which the code is going to be upstreamed must be identified:

* **(i) Upstreaming to existing components**.
When the target Project already exists in NiPreps, the Maintainers of the source project and the Maintainers of the target project must be in agreement that the proposal is adequate, and will be together responsible for overseeing the upstreaming process and for ensuring the process is finalized.
The Maintainers of both source and target Projects will operate as if they were a unique maintainers team. Therefore decisions will be consensus-based, with the possibility of initiating appeal processing to the Organization Steering Committee.
* **(ii) Upstreaming to a new project or to a new project under a sibling organization**.
The Maintainers of the source project will proceed with the proposal of a new Organization project following the above guidelines.
An example of this option will be set out by the extraction of the visual report system from *NiWorkflows* as a standalone project called *NiReports*.

In either case, the Maintainers of the source project are responsible for taking all the reasonable measures to preserve the VCS (version control system) history whenever possible, as well as ensuring the `CONTRIBUTORS.md` files of source and target projects are up-to-date and properly represent contributors.
If a contributor is to be transferred (or duplicated) into a sibling organization, they must be properly noticed.

#### 8.5. Upstreaming to other organizations

The most common case for these source code transfers will be the upstreaming of features to NiPype.
As for **8.4.ii**, the Maintainers of the source project are responsible for ensuring that the procedure is carried out correctly:

* keeping track of contributions and crediting thereof;
* communicating with the Maintainers of the receiving Project and coordinating any necessary actions;
* informing affected contributors, explicitly notifying of licensing terms changes, and aborting the upstreaming process if they do not agree with the transfer of their contributions;
* whenever possible, guide and help contributors in the process of upstreaming the code themselves;
* notify the Organization Steering Committee of the outbound code sharing action and assume any decision on the contrary, should it be issued.

## 9. Authorship and scientific publications

All end-user applications and core components have a `.main/` folder directly under the repository's root containing files and scripts to prepare author's lists before publication in scientific journals and or posting preprints or Zenodo entries.
How these resources under `.maint/` must be used is described in the `project-docs/GOVERNANCE.md` document.

End-user applications and core components that make use of other core components of the framework must include "*The NiPreps Developers*" collective of authors listed as a consortium.
All authors within the consortium must be listed in the paper, following the guidelines of the journal to the effect.
The collective of authors list is maintained in the `org-docs/COLLECTIVE-OF-AUTHORS.md` file.

## 10. Enforcement of the Code of Conduct
Instances of abusive, harassing, or otherwise unacceptable behavior may be
reported by contacting Oscar Esteban at <code@oscaresteban.es>
or Chris Markiewicz at <markiewicz@stanford.edu>, two members of the project team.

## 11. Amendments

Amendments to this charter, the antitrust policy, the trademark policy, or the code of conduct may only be made with at least a 3/4 affirmative vote of the Steering Committee.

---
Part of MVG-0.1-beta.
Made with love by GitHub. Licensed under the [CC-BY 4.0 License](https://creativecommons.org/licenses/by-sa/4.0/).
