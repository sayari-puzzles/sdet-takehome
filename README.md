#  SDET Technical Assessment

**Please be sure that you do not fork this repo, or try to commit changes to it. Once you have read this brief, go to the [setup guide](setup.md) to get started.** 

This assessment allows you to demonstrate your ability to plan and execute testing of a basic full stack component. You'll be working with a React/TypeScript frontend and a Node/Express/Postgres backend that records interactions between people.

![Screenshot 2025-04-22 at 9 34 00 AM](https://github.com/user-attachments/assets/7bdeb2ba-9050-4583-a44a-f5763511297c)

The component allows users to:
- View a list of interactions between people
- View more details of a selected interaction
- Create new interactions
- Delete existing interactions

Note that the code is not perfect and does not behave as such; not only will you be writing tests to help avoid future breaking changes, but you may also need to take note of existing bugs and issues.

***You are not expected to build an exhaustive set of test cases. When choosing which tests to write, focus on areas you deem to be the most important or interesting. If there's more that you would implement in a real word situation, make note of this in your strategy document.***

## Assessment Tasks

### Part 1: Test Automation Strategy
Create a document explaining how you would implement a complete test strategy for this component, including:
- What would be automated vs manually tested
- Additional types of testing you would recommend (performance, security, etc.)
- How you would structure test data
- Any improvements you would suggest to make the component more easily testable

Save this document to the repository.

### Part 2: API Testing

Set up an API testing framework of your choice (Jest, Mocha/Chai, Supertest, etc.) These tests should focus on direct endpoint calls.
   - Write tests for each of the API endpoints


### Part 3: Frontend Testing
Set up a UI testing framework of your choice (React Testing Library, Cypress, Playwright, etc.) These tests should focus on UI components in isolation.
   - Write at least two tests for the frontend component or one of its sub-components.

### Part 4: Integration Testing
 These tests should simulate real user interactions through the UI, hitting the actual backend. Create at least one end-to-end test that:
   - Loads the application
   - Creates a new interaction
   - Verifies it appears in the list in the UI, and in the database
   - Deletes the interaction
   - Verifies it's removed from the list in the UI, and in the database

### Part 5: Test Execution
Once your tests are written, we need a way to execute them. If you have worked with CI/CD before:
   - Update the CI configuration file (`.github/workflows/main.yml`)
   - Configure it to run your test suite
   - Note that this will require you to add repository secrets for the database credentials and connection information in that file (`POSTGRES_USER` etc)

If you do not have experience in this area, instead provide a document with instructions on how we can execute your tests.

### Part 6: Observations
You may note bugs or edge cases during this process. Note them in a document called `bugs.md` and commit it to the repo. You are not expected to find everything that might qualify as a bug in the alloted time.
   

## Deliverables
1. Test strategy document committed to the repo
2. Working test code for both frontend and backend committed to the repo
3. CI configuration file that executes your tests, or a README with instructions on how to run your work
4. Bug document committed to the repo

## Evaluation Criteria
- Code quality and organization
- Test coverage and methodology
- Handling of edge cases
- Clarity of documentation
- Implementation of automation best practices
- Ability to identify bugs and weak points

## Next Steps
Our team will evaluate your assessment. If the evaluation criteria are met, you'll be invited to attend a panel interview to discuss your assessment.
