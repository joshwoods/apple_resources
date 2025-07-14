

- App Store Connect API
- Xcode Cloud Workflows and Builds
-  Artifacts 

API Collection

# Artifacts

Read information about artifacts Xcode Cloud creates when it performs a build.

## Overview

The `ciArtifacts` resource represents an artifact that Xcode Cloud creates when it performs a workflow’s action. Use it to access the artifact’s:

- Download URL

- Filename

- File size

- Type

Use the provided information to create statistics for the artifacts Xcode Cloud creates or archive Xcode Cloud build artifacts on your own server.

Note

This resource supports JSON web tokens with a lifetime of up to six months. For more information, see Determine the Appropriate Token Lifetime.

## Topics

### Getting Build Artifact Information

Read Xcode Cloud Artifact Information

Get information about the artifact Xcode Cloud created for a specific action when it performed a build.

### Objects

object CiArtifact

The data structure that represents the output of an Xcode Cloud build action resource.

object CiArtifactResponse

A response that contains a single Artifacts resource.

## See Also

### Build Information

Build Runs

Read detailed build information and start new builds.

Build Actions

Read information about actions you configured for an Xcode Cloud workflow and their related data such as artifacts, issues, or test results.

Issues

Read information about issues that occurred when Xcode Cloud performs a build.

Test Results

Read test results for test actions Xcode Cloud performs.

