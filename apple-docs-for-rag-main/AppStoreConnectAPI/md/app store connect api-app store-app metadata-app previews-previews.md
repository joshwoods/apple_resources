

- App Store Connect API
- App Store
- App Metadata
-  App Previews 

API Collection

# App Previews

Upload and download app previews for an app locale and display target.

## Overview

An `appPreviews` resource represents a single app preview for an app locale and display target. Use this resource to:

- Upload new app previews to App Store Connect.

- Download existing app previews.

- Set a custom timestamp for the preview’s poster frame.

To upload app previews, begin by creating an App Preview Sets resource for the locale and display target. For more information, see App preview specifications.

## Topics

### Listing App Previews and Reading Information

List All App Previews for an App Preview Set

List all ordered app previews in a preview set.

Read App Preview Information

Get information about an app preview and its upload and processing status.

### Creating, Modifying, and Deleting App Previews

Create an App Preview

Add a new app preview to a preview set.

Modify an App Preview

Commit the app preview after uploading it, and update the poster frame timecode.

Delete an App Preview

Delete an app preview within a preview set.

### Objects and Data Types

object AppPreview

The data structure that represent an App Previews resource.

object AppPreviewCreateRequest

The request body you use to create an App Preview.

object AppPreviewUpdateRequest

The request body you use to update an App Preview.

object AppPreviewResponse

A response that contains a single App Previews resource.

object AppPreviewsResponse

A response that contains a list of App Preview resources.

object UploadOperation

Upload instructions for assets such as app previews and app screenshots.

type PreviewType

String that represents the display type of an app preview.

object PreviewFrameImage

The properties that describe a preview frame image for an app preview or app event video.

object AppMediaVideoState

The properties that describe the state of an app preview or app event video.

object AppMediaPreviewFrameImageState

The properties that describe the state of a preview frame image for an app preveiew or app event video.

## See Also

### Managing App Previews

Uploading App Previews

Upload your app previews, including video files, to App Store Connect by using the asset upload APIs.

Uploading Assets to App Store Connect

Upload screenshots, app previews, attachments for App Review, and routing app coverage files to App Store Connect.

App Preview Sets

Create sets of app previews to upload to App Store Connect.

