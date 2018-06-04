# QA Testing Task
Imagine the following situation. You need to establish a QA process in a cross-functional
team. The team builds a front-end application using REST APIs.
	
1. Where would you start? What would be your first steps?
<br/>**Answer**:
<br/>I will first start by sanity testing of basic cases via front-end to capture all the bugs and issues found in UI and REST API.
<br/>Later as time permits start developing automation test suite as follows: 
	1. Develop a basic skeleton for testing the REST API's.
	2. Followed by a Selenium based test suite for automating regression test cases of UI for build verification test.

2. Which process would you establish around testing new functionality? How would you
want the features to be tested?
<br/>**Answer**: 
<br/>Testing of any new functionality should adhere following steps: 
	1. Existing regression and unit test cases should pass on test environment where the functionality is deployed to avoid any integration issue impacting existing functionalities.
	2. New feature should be tested once manually to test all the edge test cases and cherry pick which cases can be added to automation test suite.
	3. Update the test suite (REST API & WEB) for relevant test cases to ensure complete sanity of the app.

3. Which tools would you suggest using to help your team with a daily work?
<br/>**Answer**: 
<br/>Following tools would aid in daily work and provide great assistance to team members: 
	1. _Central Repository (Wiki)_: To add all the project related and team related details to provide overall visibility to all the team members 
	2. _Project Management and Bug Tracking Tool_: Manage and monitor all the tasks to provide visibility of the task status across teams.
	3. _Messenger_: To provide cross team interaction and discussion about task updates and impediments.

4. If you would do a test automation which techniques or best practices would you use the
application?
<br/>**Answer**:
<br/>Following best practice should be incorporated in case of UI test automation: 
	1. Page Factory design pattern should be used to separate test action with test elements and test logic.
	2. Parameterize the domain/environment where test is to be executed to enable easy test execution on multiple environments
	3. Parallel execution of test cases on different browser/OS by ensure each test case is independent of each other.
	4. Ensure all the configurations are in one xml file to provision single source of control for all feature test.
	5. Take screenshots on failed test cases 
	6. Log all actions being performed in test execution.