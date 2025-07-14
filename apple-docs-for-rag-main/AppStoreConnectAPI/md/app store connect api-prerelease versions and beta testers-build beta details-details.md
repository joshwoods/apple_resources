

- App Store Connect API
- Prerelease Versions and Beta Testers
-  Build Beta Details 

API Collection

# Build Beta Details

TestFlight-specific information about beta builds.

## Overview

Every build has a `buildBetaDetails` resource that represents TestFlight-specific information about the build.

## Topics

### Getting Build Beta Details Information

List Build Beta Details

Find and list build beta details for all builds.

Read Build Beta Detail Information

Get a specific build beta details resource.

Read the Build Information of a Build Beta Detail

Get the build information for a specific build beta details resource.

### Modifying Build Beta Details

Modify a Build Beta Detail

Update beta test details for a specific build.

### Objects and Data Types

object BuildBetaDetail

The data structure that represents a Build Beta Details resource.

object BuildBetaDetailUpdateRequest

The request body you use to update a Build Data Detail.

object BuildBetaDetailResponse

A response that contains a single Build Beta Details resource.

object BuildBetaDetailsResponse

A response that contains a list of Build Beta Detail resources.

type ExternalBetaState

String that represents a build’s availability for external testing.

type InternalBetaState

String that represents a build’s availability for internal testing.

## See Also

### Build Resources

Builds

Manage builds for testers and submit builds for review.

Beta Build Localizations

Beta test information about builds, specific to a locale.

Build Beta Notifications

Requests to send notifications to all assigned testers that builds are ready for testing.

