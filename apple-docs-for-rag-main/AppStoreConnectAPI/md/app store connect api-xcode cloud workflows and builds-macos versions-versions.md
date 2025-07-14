

- App Store Connect API
- Xcode Cloud Workflows and Builds
-  macOS Versions 

API Collection

# macOS Versions

Read macOS version information you configure for an Xcode Cloud workflow.

## Overview

The `ciMacOsVersions` resource represents the version of macOS you configure for an Xcode Cloud workflow.

To change a workflow’s build environment, use the Workflows resource.

Note

This resource supports JSON web tokens with a lifetime of up to six months. For more information, see Determine the Appropriate Token Lifetime.

## Topics

### Getting macOS Version Information

List All macOS Versions Available in Xcode Cloud

List all macOS versions available to Xcode Cloud workflows.

Read macOS Version Information

Get information about a specific macOS version that’s available to Xcode Cloud workflows.

List Available Xcode Versions for a macOS Version

List all Xcode versions available for a specific macOS version in Xcode Cloud.

### Objects

object CiMacOsVersion

The data structure that represents a macOS Versions resource.

object CiMacOsVersionResponse

A response that contains a single macOS Versions resource.

object CiMacOsVersionsResponse

A response that contains a list of macOS Versions resources.

## See Also

### Xcode Cloud Products and Workflows

Products

Read information about the products Xcode Cloud detected or delete a product and all its associated information.

Workflows

Manage Xcode Cloud workflows and view workflow details like actions and start conditions.

Xcode Versions

Read Xcode version information you configure for an Xcode Cloud workflow.

