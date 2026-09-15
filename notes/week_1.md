# Day 1
### [[bash]] commands:

```
ls
pwd
which bash
cd / && ls  # root directories
mkdir
ll  ## long list
cd ./
cd ..
touch <file>

sudo su  # super user (root access)

echo "test string" >> <file>
cat <file>

mkdir <dir>
cp <source_path> <destination_path>
mv <source_path> <destination_path>
rm <source_path>
rm -r <directory>
```

permission blocks \[3], owner, group, user
`(d)(rwx)(r-x)(r-x)`
- d ➡ directory
- r ➡ read
- w ➡ write
- x ➡ execute
- `-x` ➡ no execute
`chmod +x <file>` ➡ make file executable

### Linux packages:

```
sudo apt-get update

sudo apt-get upgrade

sudo apt install <package>

which git   # path to the package, git example
```

### Shell script:

```
chmod +x <path_to_file>  # add executable permission
```

### Git:

```
git revert <commit_hash>  # rollback to previous commit

git reflog  # shows all actionin the git directory

git reset --hard <commit_hash>

git switch -c feature/<feature_name>  # checkout alternative

git rebase # avoid an additional merge commit
```

Head: pointer to working branch

#### Branching workflow:

- dev: merge feature branches
- stage: testing before going live
- main: always live (in production)

#### SSH for GitHub

```
shh-keygen -t ed25519 -C "example@email.com"
```

Git Games: `Oh my Git`, `learngitbranching.js.org`

# Day 2

## Jira, Agile & SDLC
```
Planning ➡ Designing ➡ Implementation ➡ Testing ➡ Maintance 

Plan ➡ Build ➡ Test ➡ Review ➡ Improve ➡ Repeat
```

### Agile
- Incremental Delivery & Collaboration
- Breakdown into smaller tasks
- Helps with every changing requirements and demands

### Jira
- Project blacklog
- Start sprints
- Sprints include development and testing
- Sprint close: sprint review. retrospect, QA report,

### Jira Basics
Tracking Tasks, Bigs, Stories & Progress 
- Projets & Issues
- Boards & Backlogs
```
Project ➡ Issue ➡ Assignee ➡ Status ➡ Completion
```
**Every issue moves through statuses as work progresses**
```
TO-DO ➡ In Progress ➡ Testing ➡ Done
```

#### User Story Structure
**Writing stories form the User's perspective**
Example: User wants to make a change in their profile without needing to contact customer support.

**Strong Story Checklist**
- Everyone should be able to understand
- Deliver meaningful outcome to the user
- Clear understandable scope the team

**What does the user need?**
- A user story explains **WHO** needs **WHAT** and **WHY**.

**Given, When, Then**
Acceptance Criteria in Practice
- Given: What is the starting situation
- When: What does the user do
- Then: What should happen?

**What does "DONE" mean?**
Clear conditions that tell us whether a story is successful.

### Test Plan Essentials
Organizing testing before execution.
- Objective & Scope
- Resource & Schedule
- Risks & Mitigation

**How will we test the feature?**
- Scope, Objectives, Test Approach
- People & Responsibilities
- Tools & Environment
- Schedule, Risks & Mitigation

### Test Case Anatomy
Components of repeatable verification steps
- Identification & Precaution
- Steps & Test Data
- Expected Design

**Test Design Techniques**
- Equivalence Partitioning
- Boundary Testing
- Decision Tables & State Testing
- Exploratory & Risk Based Testing

**How do we check the software?**
- Test ID, Module, Test Scenario
- Precondition, Test Steps, Test Data
- Expected Result & Actual Result
- Status & Evidence

### QA Lifecycle
```
Planning ➡ Test Design ➡
```
- Requirements & Planning
- Evaluation & Defects
- Closure &

#### Defect Lifecycle
Tracking defects through resolution
```
Test ➡ Defect found ➡ Open ticket, assign dev ➡ fix, retest ➡ Reopen if not fixed 
```

### Manual Testing
Human-centered verification practices. Exploratory sessions investigation.

### Automation Basics
Where automation adds value in QA Testing. Regression testing helps perform long tests. Manual testing won't be replaced.

**Scripting Practice**

### Key Takeaways
- Agile delivers value through short feedback cycles
- Jira makes work and progress visible
- User Story
- Acceptance Criteria

### Practice Agile Thinking
Apply Agile to a real feature.
- Break it down
- Prioritize by value
- Plan your sprint
- Feedback & Sharing

`saucedemo.com`
