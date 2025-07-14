

- App Store Connect API
- Xcode Cloud Workflows and Builds
-  Build Runs 

API Collection

# Build Runs

Read detailed build information and start new builds.

## Overview

The `ciBuildRuns` resource represents an Xcode Cloud build. Use it to get a list of builds Xcode Cloud performed and access detailed information for a specific build; for example:

- The status of ongoing and completed builds

- The number of issues Xcode Cloud encountered during the build

- The build number

- Start and completion dates

- Actions Xcode Cloud performed

Additionally, use the `ciBuildRuns` resource to tell Xcode Cloud to start a new build.

Note

This resource supports JSON web tokens with a lifetime of up to six months. For more information, see Determine the Appropriate Token Lifetime.

## Topics

### Getting Build Information

Read Xcode Cloud Build Information

Get information about a specific Xcode Cloud build.

List All Actions for an Xcode Cloud Build

List all actions Xcode Cloud performed during a specific build.

List All Builds Xcode Cloud Created in App Store Connect

List All App Store Connect and TestFlight Builds when it performed a build.

### Starting a New Build

Start a Build

Start a new Xcode Cloud build for a workflow.

### Objects

object CiBuildRun

The data structure that represents a Build Runs resource.

object CiBuildRunCreateRequest

The request body you use to start a new Xcode Cloud build.

object CiBuildRunResponse

A response that contains a single Build Runs resource.

object CiBuildActionsResponse

A response that contains a list of Build Actions resources.

## See Also

### Build Information

Build Actions

Read information about actions you configured for an Xcode Cloud workflow and their related data such as artifacts, issues, or test results.

Artifacts

Read information about artifacts Xcode Cloud creates when it performs a build.

Issues

Read information about issues that occurred when Xcode Cloud performs a build.

Test Results

Read test results for test actions Xcode Cloud performs.

