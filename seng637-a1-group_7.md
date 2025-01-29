>   **SENG 637 - Software Testing, Reliability, and Quality**

**Lab. Report \#1 – Introduction to Testing and Defect Tracking**

| Group: 7     |
|-----------------|
| Tobin Eberle              |   
| Tom Wilson              |   
               


# Table of Contents

[1. Introduction](#introduction)

[2. High-level description of the exploratory testing plan](#high-level-description-of-the-exploratory-testing-plan)

[3. Comparison of exploratory and manual functional testing](#comparison-of-exporatory-and-manual-functional-testing)

[4. Notes and discussion of the peer reviews of defect reports](#notes-and-discussion-of-the-peer-reviews-of-defect-reports)

[5. How the pair testing was managed and team work/effort wasdivided](#how-the-pair-testing-was-managed-and-team-workeffort-was-divided)

[6. Difficulties encountered, challenges overcome, and lessons learned](#difficulties-encountered-challenges-overcome-and-lessons-learned)

[7. Comments/feedback on the lab and lab document itself](#commentsfeedback-on-the-lab-and-lab-document-itself)

# Introduction

The purpose of this lab was to experiment with scripted/non-scripted manual exploratory testing and regression testings. Prior to this lab, we had very little experience in this area apart from non-formal, undocumented functional testing of personal projects. This report will detail our process with both the sripted/non-scripted exploratory tests, our results, and lessons/knowledge we took away.

# High-level description of the exploratory testing plan

The following sections outline the test plan which will be executed for the exploratory, manual non-scripted (EMNS) testing. 

### 1. Scope of Testing
	
The scope of testing is based on the ATM use case diagram and is split into three parts.

#### 1.1. System Startup/Shut Down
Refers to all activity involved with operator starting and stopping the system, 
entering the amount of money the ATM has, as well as the initial communication 
with the bank.

#### 1.2. User Sessions
This will encompass any initial user login functions, such as card and pin entering 
and their valid states. We will also test the persistence of the system here for a user logging in/out.

#### 1.3. Transactions
These include all the transaction types listed in the requirements: withdrawal, 
deposit, transfer, and inquiry. Additionally, because there are multiple account 
types, every transaction will need to be replicated for each. This test will have 
some overlap with 1.1, as we will need to test some of transaction functionalities 
with the amount of money existing in the ATM. Those tests will be considered 
transaction tests for our purposes.


### 2. Test Types

For this test plan, we will focus solely on functional testing. 

#### 2.1. Functional Testing
To ensure that the business logic is properly implemented we will 	
employ functional testing. These tests  will consist of ensuring that a certain ATM functionality matches its requirements.

### 3. Test Logistics

#### 3.1. Bug Tracking
Bug tracking will be done in a custom JIRA Kanban board and bugs will be 
logged with the fields as required be the lab report (for example including, initial 
conditions, expected outcome, version number, etc.).

#### 3.2. Order and timeframe 
As per the guidelines, we are time limiting all our EMNS testing to thirty minutes, 
and will test as much functionality of the ATM system as possible during this timeframe. We will proceed in numerical order of scope from 1.1 to 1.3, as this represents least possible functionalities to most. 

#### 3.3. Drivers
Testing will be done in pairs. One person will be the controller and perform the
tests on the ATM interface while the second person will log bugs in JIRA. 

# Comparison of exploratory and manual functional testing

Exploratory testing managed to find all bugs found in the manual functional testing section, along with some additional bugs not found in the manual functional testing. The informality of exploratory testing allowed for iteration of different functions in rapid succession, which gave a relatively high amount of test coverage in the allotted time, but without significant rigor in terms of knowing which tests were performed and how comprehensive the coverage had been.  Manual functional testing was very precise and, given an extensive enough test plan, would allow for a more consistent and comprehensive test coverage - although in this case the extent of the test coverage was fairly small since it was a teaching tool. Manual functional testing is slower per test case, due to the precise nature of setup and execution, and requires additional planning, but in order to produce high quality software, it is generally required. Please see the "Defect_Report_Group7.pdf" for more details on the found bugs.

# Notes and discussion of the peer reviews of defect reports

While peer reviewing defect reports, efforts were made to check for accurate and detailed information regarding, especially metadata for each test and descriptions of test initial conditions, expected result and observed result.

# How the pair testing was managed and team work/effort was divided 

Both testers took turns with one driving the operation of the ATM software and one keeping track of test conditions while entering bug reports in JIRA. The pair would both visually review the defect reports to ensure fullness and accuracy of data. The effort was divided equally between parteners.

# Difficulties encountered, challenges overcome, and lessons learned

It is helpful to determine a standard approach to documenting system state, such that the quality of the bug reports remains consistent throughout. Otherwise, ad hoc creation of bug reports by different testers may result in confusion when being interpreted in the future. It is important to include sufficient detail such that future users can easily interpret and reproduce the test cases and outcomes.

# Comments/feedback on the lab and lab document itself

This lab was an effective way to teach the general setup of a software test process and tracking plan and system, including regression.  Additionally, it highlighted the differences between exploratory and scripted testing effectively.  The ATM program was a humorous and interesting way to show a real world example of buggy software.
