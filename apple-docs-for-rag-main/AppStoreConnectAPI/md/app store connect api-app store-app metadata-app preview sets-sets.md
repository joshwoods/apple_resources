

- App Store Connect API
- App Store
- App Metadata
-  App Preview Sets 

API Collection

# App Preview Sets

Create sets of app previews to upload to App Store Connect.

## Overview

An `appPreviewSets` resource represents a collection of app previews for an app locale and display target; for example, a set of screenshots for the Simplified Chinese listing of your app for an iPhone with a 6.5” display size. Use app preview sets to:

- Begin the process of uploading app previews.

- Reorder app previews after they’re uploaded.

To upload individual previews, uses the App Previews resource.

For more information about app previews, see App information.

## Topics

### Getting Preview Sets and Reading Information

Read App Preview Set Information

Get an app preview set that includes its display target, language, and the previews it contains.

### Creating and Deleting Preview Sets

Create an App Preview Set

Add a new app preview set to an App Store version localization for a specific app preview type and display size.

Delete an App Preview Set

Delete an app preview set and all of its previews.

### Listing and Reordering All Previews in a Set

List All App Previews for an App Preview Set

List all ordered app previews in a preview set.

Get All App Preview IDs for an App Preview Set

Get the ordered app preview IDs in a preview set.

Replace All App Previews for an App Preview Set

Change the order of the app previews in a preview set.

### Objects

object AppPreviewSet

The data structure that represent an App Preview Sets resource.

object AppPreviewSetCreateRequest

The request body you use to create an App Preview Set.

object AppPreviewSetResponse

A response that contains a single App Preview Sets resource.

object AppPreviewSetsResponse

A response that contains a list of App Preview Set resources.

object AppPreviewSetAppPreviewsLinkagesRequest

A request body you use to reorder the app previews in a preview set.

object AppPreviewSetAppPreviewsLinkagesResponse

A response body that contains a list of related resource IDs.

## See Also

### Managing App Previews

Uploading App Previews

Upload your app previews, including video files, to App Store Connect by using the asset upload APIs.

Uploading Assets to App Store Connect

Upload screenshots, app previews, attachments for App Review, and routing app coverage files to App Store Connect.

App Previews

Upload and download app previews for an app locale and display target.

