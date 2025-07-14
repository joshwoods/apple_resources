

- App Store Connect API
- App Store
-  App Store Version Phased Releases 

API Collection

# App Store Version Phased Releases

Manage phased releases of updates to your app.

## Overview

`appStoreVersionPhasedReleases` handles your process of releasing app updates to customers in stages. Use this resource to set up your process for an app update. This resource is not available for the first version of an app, only for subsequent releases.

For more information, see Release a version update in phases.

## Topics

### Managing Phased Releases

Create an App Store Version Phased Release

Enable phased release for an App Store version.

Modify an App Store Version Phased Release

Pause or resume a phased release, or immediately release an app.

### Canceling Phased Releases

Delete an App Store Version Phased Release

Cancel a planned phased release that has not been started.

### Objects and Data Types

object AppStoreVersionPhasedRelease

The data structure that represent an App Store Version Phased Releases resource.

object AppStoreVersionPhasedReleaseCreateRequest

The request body you use to create an App Store Version Phased Release.

object AppStoreVersionPhasedReleaseResponse

A response that contains a single App Store Version Phased Releases resource.

object AppStoreVersionPhasedReleaseWithoutIncludesResponse

object AppStoreVersionPhasedReleaseUpdateRequest

The request body you use to update an App Store Version Phased Release.

type PhasedReleaseState

String that represents the progress of a phased release for an app version.

## See Also

### App Store Publishing

App Store Version Release Requests

Manually release an App Store approved version of your app to the App Store.

App Pre-Orders

Manage the settings that make your app available for pre-order.

App availability

Manage territory and date settings that make your app available for pre-order.

