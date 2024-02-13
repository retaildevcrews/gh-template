# Engineering Practices

## How we code together

### Branch Strategy

- `main` branch will be used
  - It will be locked, requiring a PR to make commits.
  - It will be shippable at any time.
- Branches will be used for story or bug-fix work.
  - Naming convention will include alias with a short description of the story or bug (e.g., `dsturgell-create-working-agreement` or `jofultz-deploy-script-error-on-box`)
  - Commits should always have a short but descriptive message explaining what is changing.

### Versioning & Tagging

- Code requires versioning to support side-by-side releases.
- Semantic versioning will be used (ex.: 0.5.0-MMdd-hhmm).
- We will tag as needed to identify releases along main branch.

### Reviews

- The entire team owns quality.
- While Pull Requests will be required as an official form of review for any work done, ad-hoc code reviews or design reviews are encouraged.
- Designs that may impact other areas or assumptions should be reviewed with a larger audience (preferably including the project leads) for visibility to the proposed changes and feedback.

### Pull Requests

- PRs should be small in nature; ideally should close one or more tasks.
- PRs should contain complete descriptions that follow the template and describe the scope of the work and how it meets the acceptance criteria if not obvious.
- A branch policy that requires the PR is tied to a task or bug is in place.
- A branch policy that requires one approver to complete a PR is in place. Explicitly call out the approvers as named reviewers. Ask for committed approvers early (consider asking at assignment), and as a committed approver attempt to complete within 12hours of assignment. If you don't feel you are a qualified approver, comment on that, remove the explicit reviewer assignment to yourself and try to find another approver to replace you.
- A branch policy that requires a successful and unexpired merge build before completion is in place.
- A branch policy that requires all PR comments to be resolved is in place.
- Linters must pass before completion. (Note: not all file types will require linting.)
- Tests must pass before completion.
- PRs will utilize a squash merge into main upon completion ensuring a linear commit history with a single consolidated commit per PR.
- Branches will be deleted after PR completion -- missed functionality should be captured as a new bugfix or story.

## Definition of Done

- Code changes reviewed & signed off
- Existing documentation is updated (readme, .md's)
- New documentation needed to support the change is created
- Code changes checked into main
- All existing automated tests (unit and/or e2e) pass successfully, new tests added as needed
- CI completes successfully
- CD completes successfully
- Smoke test production deployment for minimum of 2 weeks
- New changes in smoke test for 48hrs (ongoing)
- Create task for required artifacts

Engineering Playbook [Definition of Done](https://github.com/microsoft/code-with-engineering-playbook/tree/master/agile-development/team-agreements/definition-of-done/readme.md)

### Work Items

- We will track our work in GitHub
- We will prefer public repos when possible
- Our sprint work items will follow the hierarchy:  --
  - Epic
    - Story
      - Task
    - Bug
      - Task
- We will track Risk work items outside of the hierarchy so that we may easily manage them independently; however, we may choose to relate them to other work items.

|  | Sizing | Definition |
|--|--------|------------|
| **Epic** | Up to the lifetime of the project | Business initiative for a stakeholder to accomplish |
| **Story** | Completable within a sprint | Consists of multiple tasks |
| **Bug** | Completable within a sprint | Production blocking bugs are prioritized |
| **Task** | Completable within a week | Optionally defined by the story owner to help track work that must be completed to consider a story done |
| **Risk** | N/A | Something that the team would like to shine light on to ensure actions can be taken to mitigate effects on the project |

#### User Story Guidelines

> Sourced from <https://www.scrumtraining.com>

##### User Story Guideline

  Leveraging the 5 W's (who, what, when, where, why)
  
##### Acceptance Criteria/Tests

   User can *[select/operate] [Feature/Function]* so that *[output]* is *[visible/complete/etc.]*  
   Verify that...

##### I.N.V.E.S.T. in User Stories

**I**ndependent - Can it be developed independently of other stories?  
**N**egotiable - Is the scope negotiated to enable completion?  
**V**aluable - Is the value to the user or customer clear?  
**E**stimatable - Can the work be estimated? Are there unknowns, dependencies, barriers? Do we lack domain or technical knowledge?  
**S**ize appropriately - Can it be completed in the iteration?  
**T**estable - What are the tests to know the work is done?

##### User Story Issues to Avoid

- Describing a task
- UI too soon
- Write in an inactive voice
- Splitting too often in the iteration
- Thinking too far ahead
- Interdependent Stories
- Too many details
- [Gold plating](https://en.wikipedia.org/wiki/Gold_plating_(project_management))
- Stories are too small

#### Definition of Ready

- User stories clearly provide context and scope of work
- Acceptance Criteria is defined
- User stories are achievable withinin the milestone
  - Stories are broken down into prioritized tasks ranging from small to large (If extra large, break it down)
  - "Spike" if investigating something in order to timebox and track outcomes
- Story owner is able to break down user story into tasks if desired
- Dependencies identified (either external or other work items)

#### Definition of Done

- Acceptance Criteria are satisfied
- Appropriate [Pull Request template(s)](https://github.com/retaildevcrews/ngsa/blob/main/.github/PULL_REQUEST_TEMPLATE.md) satisfied
- [Pull Request](https://github.com/orgs/retaildevcrews/projects/4) approved and completed
- [DoD Review & Release](https://github.com/orgs/retaildevcrews/projects/4?card_filter_query=label%3Arelease) checklist satisfied and completed
- Demonstration recorded and available to customer (when applicable)


## Markdown (md files)

- Use [markdownlint](https://marketplace.visualstudio.com/items?itemName=DavidAnson.vscode-markdownlint) add-in for VS Code
  - Repeating header lint issues are OK if avoiding would cause readability issues
- Use [Code Spell Checker](https://github.com/streetsidesoftware/vscode-spell-checker) add-in for VS Code
- Use `-` for unordered lists
  - Mixing `-` and `*` will cause linter errors
- Use single back-quote to `call out terms`
- Add a blank line before and after ''' for visualization
- ''' blocks must specify a language for color coding
- Preview the MD to make sure it renders in a highly readable format
  - Avoid long headers, especially H1 and H2
    - Using a short Hx with a long call out renders better than a long Hx

> use call outs to emphasize important points

## Tool for Code Reviews

- CodeFlow extension for GitHub [Link](https://www.1eswiki.com/wiki/CodeFlow_integration_with_GitHub_Pull_Requests)

## Kanban Board Management Best Practices

### Triage

> All net-new issues need to be triaged, leverage Notes for discussions points as needed

- Create the issue in the appropriate repo with the appropriate template
- Add project to the issue (i.e. Helium) - this will add to the main board
  - This is only necessary in a multi-repo project like Helium
- Add all relevant tags (language, enhancement, bug, design review, etc)
- Do not add Size, Priority, Milestone, or Assignee
- All issues will be triaged at the end of the Standup call
- Add an "undo issue" for any temporary changes that need to be removed in the future

### Backlog

> Once issue has been triaged, move into the Backlog

- Once issue is triaged, add the appropriate priority label and other tags as appropriate
- Do not add size, milestone or assignee

### Sprint Backlog

> Issues identified during milestone planning will be shifted into Milestone backlog

- Need to review and update priority and add estimated sizing and milestone labels

### In Progress

> Issues that the Dev Team is actively working on

- Add assignee, size, and milestone tags & ensure all relevant tags are added
- If a design review is required, schedule meeting when moving issue to backlog
- If task is bigger than "Size:L", break into smaller tasks to ensure completion during week sprint

### PR Submitted / Review

> Pull Requests to create or update code, documentation, templates, etc and issues that need reviewed

- Complete the PR Template (ensure original issue is closed or referenced)
- Assign reviewers, assign yourself, add Project board, and Milestone
- If issue has multiple issue to close and/or reference, report each reference/close # on separate line to ensure correct link

### Done

- Issue is completed, no further action required
- Ensure task checklist is complete

### Burn Down

> During the final sprint of the milestone, create a burn down column for issues pivotal to achieve goals
