

- App Store Connect API
- App Store
-  Build Bundles 

API Collection

# Build Bundles

Read metadata for app and App Clip binaries included in a build you upload to App Store Connect.

## Overview

A `buildBundles` resource represents metadata for binaries you upload to App Store Connect as a build. It provides detailed information like capabilities an app uses, supported CPU architectures, and more. For a full list of available attributes, see BuildBundle.Attributes.

When you upload a build that contains an App Clip, use the APIs provided by the `buildBundles` resource to read:

- Cache status information for domains you associated with your App Clip

- Debug status information for domains you associated with your App Clip

- App Clip invocations you configured for testers who use the TestFlight app to launch your App Clip

- File size information for a build bundle

## Topics

### Getting Build Bundle Information

Read the App Clip Domain Cache Status Information for a Build Bundle

Get the cache status of the domain you associate with your App Clip for a specific build bundle.

Read App Clip Domain Debug Status Information for a Build Bundle

Get the debug status of the domain you associate with your App Clip for a specific build bundle.

List All Beta App Clip Invocations for a Build Bundle

Get all App Clip invocations you configure for testing for a specific build bundle.

List All File Sizes for a Build Bundle

Get all file sizes for a specific build bundle.

### Objects

object BuildBundle

The data structure that represents Build Bundles resource.

object AppClipDomainStatus

The data structure that represents the App Clip Domain Statuses resource.

object BuildBundleFileSize

The data structure that represents a Build Bundle File Sizes resource.

object AppClipDomainStatusResponse

A response that contains a single App Clip Domain Statuses resource.

object BetaAppClipInvocationsResponse

A response that contains a list of Beta App Clip Invocations resources.

object BuildBundleFileSizesResponse

A response that contains a list of Build Bundle File Sizes resources.

## See Also

### Builds

Builds

Manage builds for testers and submit builds for review.

Build Icons

Get icons from your app’s binary that are uploaded to App Store.

App Encryption Declarations

View, and assign to builds, the declarations about types of encryption used in your app.

