

- App Store Connect API
- App Store
- Custom Product Pages and Localizations
-  App Custom Product Page App Previews 

API Collection

# App Custom Product Page App Previews

Upload and download app previews for an app locale and display target.

## Overview

An `appPreviews` resource represents a single app preview for an app locale and display target. Use this resource to:

- Upload new app previews to App Store Connect.

- Download existing app previews.

- Set a custom timestamp for the preview’s poster frame.

To upload app previews, begin by using Create an App Preview Set endpoint for the locale and display target. For more information, see App preview specifications.

## Topics

### Endpoints

List All App Previews for an App Preview Set

List all ordered app previews in a preview set.

Read App Preview Information

Get information about an app preview and its upload and processing status.

Create an App Preview

Add a new app preview to a preview set.

Modify an App Preview

Commit the app preview after uploading it, and update the poster frame timecode.

Delete an App Preview

Delete an app preview within a preview set.

### Objects

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

## See Also

### Managing Custom Product Page App Previews

App Custom Product Page App Preview Sets

Create sets of app previews to upload to App Store Connect.

