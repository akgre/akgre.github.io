# Test Automation Framework

Generic open source automation framework for functional, parametric, acceptance and performance testing.

The objective is to provide a system to manage test sequences for simplifying test workflow, product analysis and troubleshooting.

## Purpose

Often when I come across applications that are for testing they are built from the ground up. It start with the goal of automating a small task and it grows to the point where it take up nearly all your time to modify, maintain and usually has different variants for multiple task. The applications are still very useful, however, without the use of a common structure any changes need to be repeated and keeping track of this can be a source of frustration.

The solution to organising the test applications would be a test management platform. TestStand is a powerful application for creating sequences and has many features, and the Robot Framework is open source and base on python, however, the former has a high cost and the later is more designed for web testing.

This is where the test automation framework comes into play. I wanted to create a test management platform that is simple to use and easy to develop with.

## Flow Overview

![high_level_flowchart](C:\Users\Zircon\Desktop\python_projects\TCM\docs\img\high_level_flowchart.PNG)

### Initiating The Session

* **Build Session:** A GUI is available for a user to select a set of tasks to perform. The session will load the selected configuration, build the session archive and load the performing module that will perform a specific task.
* **Verify Session Data:** A session could have a single set of parameters or a matrix of hundreds of permutations (there is no limit) so it is important to check the input data is valid. the data is sent to a validation function in the performing module and will notify the user of invalid entries.
* **Verify Interfaces:**  Checks that all the hardware needed for performing the task is available and will notify the user of unavailable hardware.

### Main Performing Loop

The performing function will require a set of parameters for performing the task and these parameters will be set in a definition record. The creator of the definitions can also group definitions by certain criteria which can be placed into a definition batch file.

* **Definition Batch:** List of definition batches to be performed.
* **Definition Record:** List of the records in the current batch.
* **Perform Function:** Specific module that will be performing the task and return the results.

### Session Wrap Up
* **Safe State Shutdown:** To prevent any data loss and to make sure the device under test can be removed.
* **Session Analysis:** Will display a report of the session
* **Release Data:** The user can choose to Release the data for review by other members of the team.
