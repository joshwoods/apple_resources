

- App Store Connect API
- App Store
-  Build Icons 

API Collection

# Build Icons

Get icons from your app’s binary that are uploaded to App Store.

## Overview

Use `buildIcons` to identify which icons were uploaded to App Store Connect inside your app’s binary. This is a read-only resource. For a list of supported icon asset types, see IconAssetType.

## Topics

### Getting Metadata and Downloading Icons

List All Icons for a Build

List all the icons for various platforms delivered with a build.

### Objects and Types

object BuildIcon

The data structure that represents the Build Icons resource.

object BuildIconsResponse

A response that contains a list of Build Icon resources.

object BuildIconsWithoutIncludesResponse

object ImageAsset

An image asset, including its height, width, and template URL.

type IconAssetType

String that represents the type of icon contained in the build.

## See Also

### Builds

Builds

Manage builds for testers and submit builds for review.

Build Bundles

Read metadata for app and App Clip binaries included in a build you upload to App Store Connect.

App Encryption Declarations

View, and assign to builds, the declarations about types of encryption used in your app.

