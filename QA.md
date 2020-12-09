# QA Roadmap


## Terminology

STLC - Software Testing Life Cycle

SDLC - Software Development Life Cycle

TDD - Test Driven Development

BDD - Behaviour Driven Development

RPA - Robotoci Process Automation

## Fundametals

- Testing Strategies
  - White Box Testing 
  - Gray Box Testing
  - Black Box Testing

- Testing Types
  - Code Based Tests (Unit, Integration)
  - Smoke Testing
  - Regression Testing (Sanity Testing)
  - User Acceptance
  - Performance testing (volume, stress)

- STLC Managment
  Tools which help QA engineers develop their test plan and write out test cases.

  Common tools:
    - Testlink
    - qTest
    - Testrail 

- Project Managment
  QA engineers need to report their works to higher ups and developers. There are many common task applications that can be used for that purpose:

  - GitHub Issues
  - Jira
  - Asana
  - Trello


- Methodologies
  Depending on the team we can apply different approaches to how QA testing is done. Testers should try to follow the same approach as the developers do.

  Some of those approaches would be:
  - V Model - sequential testing
  - Agile Model - Sync and iterative testing
  - Waterfall Model - Hand-off approach


## Manual Testing

Manual testing is the core fundamental of testing on which future automation and continous development is build on. Both development and test automation rely on a solid foundation laid within the manual testing plan.

A recommended way of starting off manual testing is trough Data-driven Testing, in which tester have a set of inputs and a set of expected outpus to compare actual results to which allows clean tracking in the test phase.


- TDD 

  Development againts testing. For a developer it is a huge help to know all the cases he/she needs to cover when developing a feature. Based on the project manager's description, QA developers can set up a list of test cases for a feature for developers which they can reference during development. (Test first then code approach)

- Test planing

  Ad hoc testing is a quick start point but problematic in the long run. QA engineers need to define a plan/strategy by which they will handle testing. The main question test plans answers is `How are we going to test it`.

- Test cases and scenarios

  Cases and scenarios are a list of all use cases a customer can do while using the application. They list all possible actions someone can perform on a feature. We can have cases where we test exepcted behaviour for happy inputs as well as test cases where we throw in dirty or no input at all to ensure the applications works under both conditions (user is using it properly, user is using it improperly)

- Compatibility

  As a QA engeneer you need to understand the test cases you are going by and be able to see possible scenarios that developers do not see

- Reporting

  A huge part of testing is reporting the coverage. Before shipping the application leads and project managers need to revise QA reports to determine if the current build is stable enough to be available to the customers.

- Verification and Validation

  Based on the testing results and reports QA engineers can do

  - Verification: testing that your product meets the specifications - client requirements.
  
    Question answered: Did we implement all needed features?

  - Validation: assuring that the required business logic is according to the clients requirements

    Question answered: Did we implement this feature properly? 



## Automated Testing

Branches
  - API automation test
  - Mobile automation test
  - Web automation test

<br>

- General tools
  - Selenium IDE: Open source record and playback test automation for the web
  - Ghost Inspector - automated website testing and monitoring service that checks for problems with your website or application


### API and DB testing

Usually web testing will cover test on API, but we can add API specific testing to add another layer of security in our softwares quality.

For this we can make use of applications and libraries.

Applications: 
  - Postman
  - Insomnia
  - CLI (curl)
  - RunScope

Libraries and frameworks*:
  - Cypress
  - Protractor
  - Robot
  - CodeCeption

* Librarires can often be language specific and you should use the library that fits your needs and language


### Browser and web testing

This includes E2E and UI tests which cover most ground and are the most essential. 

UI tests are very fragile in implementation if test design phase was not done properly, but they are the closest live scenario simulation.

Selenium based tools:
  - Protractor
  - Robot
  - Nightwatch

Selenium-less tools:
  - Cypress
  - Puppeteer
  - Jest

Headless browsers: 
  - Phantom JS
  - PHP browser


### Mobile app testing

For automated testing on mobile applications we can use native automation frameworks.

- Appium
- Detox
- Macaca JS



### Non functional tests

Aside from features we need to test our applications for performance.

Here we cover two issues:

- How robust is our app under pressure and where we spike in performance (Stress test) 
- How good can our app handle large requests (Volume test)


For this we can use many language native libraries, but some standard tools are:

- Jmeter
- Gatling
- Vegeta


## Next steps

This guide offers some basic info about different branches in QA testing. The roadmap is not strict and open for expansion and completing it does not mean QA mastery. From here improvement is self focused. So keep learning.