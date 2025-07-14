

- App Store Connect API
- Xcode Cloud Workflows and Builds
-  Xcode Versions 

API Collection

# Xcode Versions

Read Xcode version information you configure for an Xcode Cloud workflow.

## Overview

The `ciXcodeVersions` resource represents the version of Xcode you configure for an Xcode Cloud workflow.

To change a workflow’s build environment, use the Workflows resource.

Note

This resource supports JSON web tokens with a lifetime of up to six months. For more information, see Determine the Appropriate Token Lifetime.

## Topics

### Getting Xcode Version Information

List All Xcode Versions Available in Xcode Cloud

List all Xcode versions that are available to Xcode Cloud workflows.

Read Xcode Version Information

Get information about a specific Xcode version that’s available to Xcode Cloud workflows.

List Available macOS Versions for an Xcode Version

List all macOS versions available in Xcode Cloud that support a specific Xcode version.

### Objects

object CiXcodeVersion

The data structure that represents an Xcode Versions resource.

object CiXcodeVersionResponse

A response that contains a single Xcode Versions resource.

object CiXcodeVersionsResponse

A response that contains a list of Xcode Versions resources.

## See Also

### Xcode Cloud Products and Workflows

Products

Read information about the products Xcode Cloud detected or delete a product and all its associated information.

Workflows

Manage Xcode Cloud workflows and view workflow details like actions and start conditions.

macOS Versions

Read macOS version information you configure for an Xcode Cloud workflow.

