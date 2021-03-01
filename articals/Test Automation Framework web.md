# Test Automation Framework

## Your Solution
Product parametric, acceptance, and performance testing for based on a flexible, cost effective independent and future orientated generic open-source automation framework.

## Objective
To provide a system to meet your current and future requirements to manage test sequences, simplifying test workflow, data recording, product analysis and troubleshooting.

## Purpose

Typically test applications develop from basic essential functions, growing over time to cover variants and multiple tasks along with further aspects for certification and reliability criteria. The applications are very useful, however, without the use of a common structure the system will take up nearly all your time, and can be a source of frustration to continuous modify, maintain and document.

The ideal solution to organising the test applications is a test management platform. Current applications are either costly and require a licence for each system and comparable open source software are tailored for web or program testing.

This is where the test automation framework comes into play. I can offer a test management platform that is simple to use and easy to develop with.

## Flow Overview

![high_level_flowchart](C:\Users\Zircon\Desktop\python_projects\TCM\docs\img\high_level_flowchart.PNG)

### Initiating The Session

* **Build Session:** A GUI is available for a user to select a set of tasks to perform. The session will load the selected configuration, build the session archive and load the performing module that will perform a specific task.
* **Verify Session Data:** A session could have a single set of parameters or a matrix of hundreds of permutations (there is no limit) so it is important to check the input data is valid. The data is sent to a validation function in the performing module and will notify the user of invalid entries.
* **Verify Interfaces:**  Checks that all the hardware needed for performing the task is available and will notify the user of unavailable hardware.

### Main Performing Loop

The performing function will require a set of parameters for performing the task and these parameters will be set in a definition record. The creator of the definitions can also group definitions by certain criteria which can be placed into a definition batch file.

* **Definition Batch:** Current definition batch from the list of batches to be performed.
* **Definition Record:** Current record from the list in the current batch.
* **Perform Function:** Specific module that will be performing the task and return the results.

### Session Wrap Up
* **Safe State Shutdown:** To prevent any data loss and to make sure the device under test can be removed.
* **Session Analysis:** Will display a report of the session
* **Release Data:** The user can choose to release the data for review by other members of the team.

## Usage
### Session Queue
When the user starts the application they are presented with a queue window.

![test_queue_viewer](C:\Users\Zircon\Desktop\python_projects\TCM\docs\img\test_queue_viewer.PNG)

This application is able to queue multiple sessions and shows the user the details of the selected tests they wish to run.

![test_queue_viewer](C:\Users\Zircon\Desktop\python_projects\TCM\docs\img\test_queue.PNG)

Having a queue rather than a single selection allows the user to run the same test multiple times or build a series of smaller test sessions. The choice will be down to preference of how long the tests might take or how the users would like the tests reported.

The **setup files** have been created by the test developer; the user selects a file and the details will be displayed. The user can modify the details and save it as a new setup file.

### Session Monitor

Being able to very quickly understand where the session is as vitally important when it comes to more complex test systems. When failures are found being able to quickly discover where the issue is occurring can save huge amounts of time in solving the issue. 

When the session is running the user will be able to view the progress and control the session with the monitor.

![test_flow_monitor](C:\Users\Zircon\Desktop\python_projects\TCM\docs\img\test_flow_monitor.PNG)
