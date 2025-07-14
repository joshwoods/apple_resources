

- App Store Connect API
- App Store
-  Builds 

API Collection

# Builds

Manage builds for testers and submit builds for review.

## Overview

A `builds` resource represents a single build of an app. You must upload builds using Xcode or Transporter. Once App Store Connect processes the build, it will appear as a build resource.

Once the build is in the system, you can use the API to perform actions like:

- Submitting builds for review.

- Individually assigning builds to testers.

- Adding the build to a beta group for testing.

## Topics

### Getting Build Information

List Builds

Find and list builds for all apps in App Store Connect.

Read Build Information

Get information about a specific build.

Read the App Information of a Build

Get the app information for a specific build.

Read the App Store Version Information of a Build

Get the App Store version of a specific build.

Read the Prerelease Version of a Build

Get the prerelease version for a specific build.

Read usage metrics for a beta build

Get usage metrics for a specific build.

### Modifying Builds

Modify a Build

Expire a build or change its encryption exemption setting.

Assign the App Encryption Declaration for a Build

Assign an app encryption declaration to a build.

Deprecated

### Adding and Removing Build Access

Add Access for Beta Groups to a Build

Add or create a beta group to a build to enable testing.

Remove Access for Beta Groups to a Build

Remove access to a specific build for all beta testers in one or more beta groups.

Assign Individual Testers to a Build

Enable a beta tester who is not a part of a beta group to test a build.

Remove Individual Testers from a Build

Remove access to test a specific build from one or more individually assigned testers.

### Listing Individually Assigned Beta Testers

List All Individual Testers for a Build

Get a list of beta testers individually assigned to a build.

Get All Resource IDs of Individual Testers for a Build

Get a list of resource IDs of individual testers associated with a build.

### Checking Beta Review Submission Status

Read the Beta App Review Submission of a Build

Get the beta app review submission status for a specific build.

### Getting Information Associated with Builds

Read the Build Beta Details Information of a Build

Get the beta test details for a specific build.

Read the App Encryption Declaration of a Build

Read an app encryption declaration associated with a specific build.

Get the App Encryption Declaration ID for a Build

Get the beta app encryption declaration resource ID associated with a build.

List All Beta Build Localizations of a Build

Get a list of localized beta test information for a specific build.

### Objects

object Build

The data structure that represents a Builds resource.

object BuildResponse

A response that contains a single Builds resource.

object BuildWithoutIncludesResponse

object BuildsResponse

A response that contains a list of Builds resources.

object BuildsWithoutIncludesResponse

object BuildUpdateRequest

The request body you use to update a Build.

object BuildAppEncryptionDeclarationLinkageRequest

The request body you use to attach an app encryption declaration to a build.

object BuildAppEncryptionDeclarationLinkageResponse

A response body that contains the ID of a single related resource.

object BuildIndividualTestersLinkagesRequest

A request body you use to add or remove a build from multiple beta groups.

object BuildIndividualTestersLinkagesResponse

A response body that contains a list of related resource IDs.

object BuildBetaGroupsLinkagesRequest

A request body you use to add or remove beta groups from a build.

object ImageAsset

An image asset, including its height, width, and template URL.

object BetaBuildUsagesV1MetricResponse

A response that contains one or more beta build metric resources.

## See Also

### Builds

Build Bundles

Read metadata for app and App Clip binaries included in a build you upload to App Store Connect.

Build Icons

Get icons from your app’s binary that are uploaded to App Store.

App Encryption Declarations

View, and assign to builds, the declarations about types of encryption used in your app.

