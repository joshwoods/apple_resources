

- App Store Connect API
- App Store
- App Metadata
-  Routing App Coverages 

API Collection

# Routing App Coverages

Manage geographic coverage files for apps that use location to provide routing information.

## Overview

Use `routingAppCoverages` to upload, replace, or delete a geographic coverage file for App Review. If your app uses location to provide routing information, you must supply a geographic coverage file before submitting your app to App Review. For more information see Upload a geographic coverage file for a routing app (iOS, watchOS).

For information about creating a geographic coverage file, see “Specifying the Geographic Coverage File Contents” in Location and Maps Programming Guide.

## Topics

### Reading and Creating Routing App Coverages

Read the Routing App Coverage Information of an App Store Version

Get the routing app coverage file that is associated with a specific App Store version

Read Routing App Coverage Information

Get information about the routing app coverage file and its upload and processing status.

Create a Routing App Coverage

Attach a routing app coverage file to an App Store version.

### Modifying and Deleting Routing App Coverages

Modify a Routing App Coverage

Commit a routing app coverage file after uploading it.

Delete a Routing App Coverage

Delete the routing app coverage file that is associated with a version.

### Objects

object RoutingAppCoverage

The data structure that represents the Routing App Coverages resource.

object RoutingAppCoverageWithoutIncludesResponse

object RoutingAppCoverageCreateRequest

The request body you use to create a Routing App Coverage.

object RoutingAppCoverageResponse

A response that contains a single Routing App Coverages resource.

object RoutingAppCoverageUpdateRequest

The request body you use to update a Routing App Coverage.

object AppMediaStateError

An error code and description.

object AppMediaAssetState

The state of an app or media upload, including any errors and warnings.

## See Also

### Managing App Information and Versions

App Infos

Manage or read the app metadata that applies across all versions of your app.

App Info Localizations

Manage the app metadata that is localized and appears on the App Store.

App Store Versions

Manage versions of your app that are available in App Store.

App Store Version Localizations

Create and maintain version-specific App Store metadata that’s localized.

