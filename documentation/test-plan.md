##Overview:

- What is Test Documentation?
- Why Test Formality?
- Examples of Test Documentation
- Best practice to Achieve Test Documentation
- Advantages of Test Documentation
- Disadvantages of Test Documentation
- Scenario Testing
- Purpose, pros and cons of Scenario Testing
- Steps and tips on how to write scenario testing
- Test cases and how to write them


Test documentation is a test of arifacts created before and during the testing of the software with the purpose to estimate the effort, 
test the coverage of test we are about to perform, tracking the resource we need for testing and tracking the execution progress.
Consists of test planning, test design and test execution. 
There are 8 examples we have in test documentation:
1. Test policy - high level document which describer methods, principles and testing goals of the organisation.
2. Test strategy - a high level document which identifies the test levels to be executed for the project.
3. Test plan - a complete planning document which contains the scope, approach, resources and schedule.
4. Requirements traceability matrix - a document which connects the requirements to the test cases.
5. Test scenarios -  an item or an event of a software system which could be verified by one or more test cases.
6. Test case -  group of input values, execution, preconditions and results that are developed from test scenarios.
7. Test data - exists before the test is executed and using test data, the test cases are executed.
8. Defects report - documented report of any flaw in software system


### Advantages:
 - to either reduce or remove any uncertainties about the testing activities
 - acts as training material to freshers in the software testing process
 - good marketing & sales strategy to showcase Test Documentation to exhibit a mature testing process
 - offer a quality product to the client within specific time limits
 - helps you to improve transparency with the client

 ### Disadvantages:
 - cost of the documentation may surpass its value
 - it is time consuming
 - could be written by someone who does not know the material well
 - it canget tiring to keep the track of the changes made
 - poor documentation directly reflects the quality of the product 

 ## TEST SCENARIOS

 steps on how to write it:
 1. Read the Requirement Documents
 2. figure out possible users actions and objectives
 3. After reading the Requirements Document and doing your due Analysis, list out different test scenarios that verify each feature of the software
 4. Traceability matrix
 5. Reviewing

 Examples of test plan for STLC

 ## References: 
 https://www.youtube.com/watch?v=VPnWoroH7yA
 https://www.youtube.com/watch?v=iWtxEDE1IR4
 

 ### Whitebox testing
 Refers to a scenario where (as opposed to black box testing), the tester deeply understands the inner workings of the system or system component being tested.

## The key principles that assist you in executing white box tests successfully are:

- Statement Coverage – ensure every single line of code is tested.
- Branch Coverage – ensure every branch (e.g. true or false) is tested.
- Path Coverage – ensure all possible paths are tested.

## Why is White Box Testing necessary?
Simply because of what it is designed to do – i.e., test all possible scenarios that a system can encounter. By testing at the source code-level, a tester will be able to run through every single permutation and combination that the program can theoretically spew out.

When testing happens at such granular level, this then brings any possible defects out in the open. And your team will have an opportunity to evaluate whether some or all of them need to be fixed.

## Advantages:
White-box testing is one of the two biggest testing methods that are used today. It has several major advantages:
1. The side effects of having knowledge of the source code are beneficial to thorough testing,
2. Optimization of code becomes easy as inconspicuous bottlenecks are exposed.
3. Gives the programmer introspection because developers carefully describe any new implementation.
4. Provides traceability of tests from the source, thereby allowing future changes to the source to be easily captured in the newly added or modified tests.
5. Easy to automate.
6. Provides clear, engineering-based rules for when to stop testing.

## Disadvantages:
Even that white-box testing has great advantages, it is not perfect and contains some disadvantages. That disadvantages are:
1. White-box testing brings complexity to testing because the tester must have knowledge of the program, or the test team needs to have at least one very good programmer who can understand the program at the code level. White-box testing requires a programmer with a high level of knowledge due to the complexity of the level of testing that needs to be done.
2. On some occasions, it is not realistic to be able to test every single existing condition of the application and some conditions will be untested.
3. The tests focus on the software as it exists, and missing functionality may not be discovered.
4. The resulting test can be fragile because they are tightly coupled to the specific implementation of the thing being tested. The code under test could be rewritten to implement the same functionality in a different way that invalidates the assumptions baked into the test. This could result in tests that fail unnecessarily or, in the worst case, tests that now give false positives and mask errors in the code.

## Types of White Box Testing
White box testing encompasses several testing types used to evaluate the usability of an application, block of code or specific software package. There are listed below --

- Unit Testing: It is often the first type (first level) of testing done on an application. Unit Testing is performed on each unit or block of code as it is developed. Unit Testing is essentially done by the programmer. As a software developer, you develop a few lines of code, a single function or an object and test it to make sure it works before continuing Unit Testing helps identify a majority of bugs, early in the software development lifecycle. Bugs identified in this stage are cheaper and easy to fix.

- Testing for Memory Leaks: Memory leaks are leading causes of slower running applications. A QA specialist who is experienced at detecting memory leaks is essential in cases where you have a slow running software application.

- White Box Penetration Testing: In this testing, the tester/developer has full information of the application's source code, detailed network information, IP addresses involved and all server information the application runs on.  The aim is to attack the code from several angles to expose security threats
- White Box Mutation Testing: Mutation testing is often used to discover the best coding techniques to use for expanding a software solution.

## What Does White Box Testing Focus On?
White box tests can focus on discovering any of the following problems with an application’s code:

1. Security gaps and vulnerabilities — checking to see if security best practices were applied when coding the application, and if the code is vulnerable to known security threats and exploits.
2. Broken or poorly structured paths — identifying conditional logic that is redundant, broken or inefficient.
3. Expected output — executing all possible inputs to a function to see if it always returns the expected result.
4. Loop testing — checking single loops, concatenated loops and nested loops for efficiency, conditional logic, and correct handling of local and global variables.
5. Data Flow Testing (DFT) — tracking variables and their values as they pass through the code to find variables that are not correctly initialized, declared but never used, or incorrectly manipulated.

Within code coverage, it is possible to verify how much of an application’s logic is actually executed and tested by the unit test suite, using concepts like statement coverage, branch coverage, and path coverage. These concepts are discussed in more detail below.

- Statement Coverage
Statement coverage is a white box testing technique that ensures all executable statements in the code are run and tested at least once. For example, if there are several conditions in a block of code, each of which is used for a certain range of inputs, the test should execute each and every range of inputs, to ensure all lines of code are actually executed.

- Branch Coverage
Branch coverage maps the code into branches of conditional logic, and ensures that each and every branch is covered by unit tests.

- Path Coverage
Path coverage is concerned with linearly independent paths through the code by drawing graphs.
