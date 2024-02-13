# Working Agreement

## Goal

This living document represents the principles and expected behavior of everyone involved in the project. It is not meant to be exhaustive nor  complete. The team should be accountable to these standards and revisit, review, and revise at the start of each new engagement. The agreement is signed off by everyone.

## Code of Conduct

We pledge to follow the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/):

- **Be friendly and patient**: Remember you might not be communicating in someone else's primary spoken or programming language, and others may not have your level of understanding.
- **Be welcoming**: Our communities welcome and support people of all backgrounds and identities. This includes, but is not limited to members of any race, ethnicity, culture, national origin, color, immigration status, social and economic class, educational level, sex, sexual orientation, gender identity and expression, age, size, family status, political belief, religion, and mental and physical ability.
- **Be respectful**: We are a world-wide community of professionals, and we conduct ourselves professionally. Disagreement is no excuse for poor behavior and poor manners. Disrespectful and unacceptable behavior includes, but is not limited to:
  - Violent threats or language.
  - Discriminatory or derogatory jokes and language.
  - Posting sexually explicit or violent material.
  - Posting, or threatening to post, people's personally identifying information ("doxing").
  - Insults, especially those using discriminatory terms or slurs.
  - Behavior that could be perceived as sexual attention.
  - Advocating for or encouraging any of the above behaviors.
- **Understand disagreements**: Disagreements, both social and technical, are useful learning opportunities. Seek to understand the other viewpoints and resolve differences constructively.
- This code is not exhaustive or complete. It serves to capture our common understanding of a productive, collaborative environment. We expect the code to be followed in spirit as much as in the letter.

## How we work together

Teams and feature crews should feel free to be flexible based on your life situation - especially during COVID. Many of us work split schedules to accomodate our personal lives and health. You should feel empowered to work "your" schedule. 

### Model, Coach, Care

We should personally practice a growth mindset with three skills in particular: active role modeling, coaching others to be active role models, and showing care about team members and their personal growth.

We should all display accountability, integrity, and respect.

At every level, we practice Two-in-a-Box project management. If something is not right, you have permission to hold leads accountable. If you see something, say something.

### Timezones

Our crews are distributed across timezones and across the world. Where possible, we will have ceremonies and meetings at a time convenient to everyone. Where it's not possible, we will do our best to share the timezone tax. We don't currently have "core hours" but may consider implementing them in the future.

### How we track and share information

- We will prefer our Teams General Channel for discussions or questions over email
- We will use Teams for meetings and calls
- Teams and email communication are asynchronous, especially with crews based in different regions
- We will make documentation accessible:
  | Type | Where? | Examples |
  |------|--------|----------|
  | Organization Artifacts | ArtifactHub | Game Plan, SDD, draft documents |
  | Project Artifacts | Teams Channel Files | ADS agenda, Sprint Review videos, Meeting Notes |
  | Project Documentation | GitHub Repo | Working Agreement, code of conduct, high-level overview |
  | Architecture / Designs | GitHub Repo| Technical Design documents |

## How we plan together


### Backlogs and (Dash)boards

- Product Owner owns the Product Backlog.
- Tech Lead owns the Risk Backlog.
- User Story Board will be used to track User Story progress.
- Kanban Board will be used to track project progress
  - Board columns:
    - **Triage**: All net-new tasks/bugs/features/stories need to be created as an "issue"; things to discuss/notes can be added as a "note"
    - **Backlog**: Stories and tasks that have been refined, triaged, and prioritized.
    - **Sprint Goals**: Stories that have been committed for the current sprint.
    - **Sprint Backlog**:  Tasks that have been committed for the current sprint.
    - **In Progress**: A development team member owns the story or bug and begins work.
    - **PR Submitted/In Review**: The owner of the story or bug determines the item meets our Definition of Done and has created a Pull Request. The item will stay in this status through the PR process -- including addressing requested feedback or fixing issues found.
    - **Done**: The Pull Request/Task has completed, and the work has been committed to the `main` branch of the project repository.

### Estimating

- We will estimate User Stories with size tagging to help gauge how much work we commit to within a sprint.
- We will use T-shirts sizing for our estimation -- with XS <1 day, Small is 1-2 days, Medium is 2-3 days, Large is 4-5 days, and XL > week, needs decomposed.

### Ceremonies

- Our sprints will be one week and run from Wednesday - Tuesday with Review, Retrospective, and Planning occurring back-to-back.
- We will use an assigned Scrum Master versus rotating the role among the team.

|  | When | Length | Participants | Purpose |
|------|------|--------|--------------|---------|
| **Standup** | Monday, Wednesday, Thursday  @ 1PM CST | 10 minutes | Development Team, Scrum Master, Product Owner | Those with committed work answer: What did I do yesterday? What will I do today? Is there anything in my way? |
| **Triage** | Monday, Wednesday, Thursday  @ 1:10PM CST | 10 minutes | Development Team, Scrum Master, Product Owner| Review an net-new issues for prioritization and discussion |
| **Review** | Tuesday @ 4:00PM CST | 30 minutes | Development Team, Scrum Master, Product Owner | Demonstrate the work we did this week. Show and tell time. |
| **Retrospective** | Tuesday @ 4:30PM CST | 30 minutes | Development Team, Scrum Master, Product Owner | Reflect as a team on how we're doing -- what's working well for us, and what could we do better? |
| **Planning** | Wednesday @ 5:00PM | 30 minutes | Scrum Master, Product Owner, Development Team | Commit to work for the next sprint. |


### Pairing

Pairing work is recommended to support knowledge sharing between the team members. Work items have a dedicated field *Pairing with* so that a second team members is explicitly assigned. Each team member should look for pairing opportunities before picking up a new work item. Commits should be made by the people that are assigned to the story. Other team members are encouraged to provide feedback using PR comments.

### Sharing

Sharing is caring. We will record demos to share early and share often. We will share as we go and not wait until the end of the project.