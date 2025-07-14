

- App Store Connect API
- Xcode Cloud Workflows and Builds
-  Issues 

API Collection

# Issues

Read information about issues that occurred when Xcode Cloud performs a build.

## Overview

The `ciIssues` resource represents issues that occur when Xcode Cloud performs a build. Use it to access a list of issues that occurred and read detailed issue information; for example:

- The type of issue that occurred

- The location in your code where the issue occurred

- A message describing the issue

Note

This resource supports JSON web tokens with a lifetime of up to six months. For more information, see Determine the Appropriate Token Lifetime.

## Topics

### Getting Xcode Cloud Build Issues

Read Xcode Cloud Issue Information

Get information about a specific issue that occurred when Xcode Cloud performed a build.

### Objects

object CiIssue

The data structure that represents an Issues resource.

object FileLocation

The data structure that represents a File Locations resource.

object CiIssueResponse

A response that contains a single Issues resource.

## See Also

### Build Information

Build Runs

Read detailed build information and start new builds.

Build Actions

Read information about actions you configured for an Xcode Cloud workflow and their related data such as artifacts, issues, or test results.

Artifacts

Read information about artifacts Xcode Cloud creates when it performs a build.

Test Results

Read test results for test actions Xcode Cloud performs.

