

- App Store Connect API
- Xcode Cloud Workflows and Builds
-  Test Results 

API Collection

# Test Results

Read test results for test actions Xcode Cloud performs.

## Overview

The `ciTestResult` resource represents the test results that Xcode Cloud makes available if you configure a workflow to include a test action. Use this resource to access:

- The name of the test class

- Test file information

- The name and operating system version of the simulated device that Xcode Cloud used to perform the tests

- The time it took to run the tests

- Test status information

- A unique identifier for the tests Xcode Cloud ran

Note

This resource supports JSON web tokens with a lifetime of up to six months. For more information, see Determine the Appropriate Token Lifetime.

## Topics

### Getting Test Results

Read Test Result Information

Get a specific test result Xcode Cloud created when it performed a build with a test action.

### Objects and Types

object CiTestResult

The data structure that represents a Test Results resource.

object CiTestResultResponse

A response that contains a single Test Results resource.

## See Also

### Build Information

Build Runs

Read detailed build information and start new builds.

Build Actions

Read information about actions you configured for an Xcode Cloud workflow and their related data such as artifacts, issues, or test results.

Artifacts

Read information about artifacts Xcode Cloud creates when it performs a build.

Issues

Read information about issues that occurred when Xcode Cloud performs a build.

