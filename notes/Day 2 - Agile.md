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
Requirement Analysis ➡ Test Planning ➡ Test Design ➡ Test  Environment setup ➡ Test Execution ➡ Test Reporting ➡ Defect Tracking ➡ Test Closure
```
- Requirements & Planning
- Evaluation & Defects
- Closure & Lession

#### Defect Lifecycle
Tracking defects through resolution
```
Test ➡ Defect found ➡ Open ticket & assign dev ➡ fix & retest ➡ Reopen if not fixed or close
```

### [[Manual Testing]]
Human-centered verification practices. Exploratory sessions investigation.

### [[Automation]] Basics
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

Test login page of : `saucedemo.com`
Inner page test:
- sub categories of Dynamic Catalog: items not clickable
- Lazy load page: infinite scroll
- Products: no option for item quantity
- Mouse cursor doesn't change to pointer when hovering over cart
- Pressing enter while filling checkout details reverts to cart page
- Allows checkout and invoice generation without any items
- Checkout details only requires 1 character each in the input fields
- Items in cart persist through different users
- Item named "Test.allTheThings()", item description "carry.allTheThings()"
- Items filter dropdown doesn't work on the arrow.
- Token expiration in 7-10 minutes even with action:
	![[Pasted image 20260915145643.png | 300]]
- Going backwards after logging in can lead to the login page allowing another login credential to be used
- visual_user: has scrambled UI components
- error_user: doesn't take lastname in checkout, and finish checkout button doesn't work
- problem_user: last name enters on first name field. doesn't allow checkout ure to missing last name

**Jira Ticket**
- Title: Feature/User Login
- Description: Allow users to login with registered credentials or Google/Apple account OAuth.
- User Story: As a user when I open a the website, I should be greeted with the login page where a username and password input fields are present along with google or apple account login option as well. Entering valid credentials or OAuth login should lead to the home page of the website. If I use invalid credentials, I should get descriptive error messages depending on the action.
- Acceptance Criteria:
	- Usernames must be between 4-32 characters long, and only allow \[A-Za-z, 0-9, \_, @]
	- password must be between 8-16 characters, only allow \[A-Za-z, 0-9, \_, @]
	- Logging in with empty input fields should display "Please enter username and password" error message and for either username or password accordingly.
	- Invalid username should display "Username not found" and Invalid password should display "Invalid password" error messages.
	- OAuth login should connect seamlessly.
	- There should be an option "Forgot password" to reset password.
	- There should be an option "Not a user? Register here" that leads to the registration page.
	- If an already logged in person goes to the login page, they should be redirected to the home page.

## Automation Basics
Applies both in SDLC and STLC
- Playwright
- POM