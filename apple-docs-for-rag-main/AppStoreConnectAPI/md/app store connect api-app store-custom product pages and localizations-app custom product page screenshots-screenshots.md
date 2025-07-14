

- App Store Connect API
- App Store
- Custom Product Pages and Localizations
-  App Custom Product Page Screenshots 

API Collection

# App Custom Product Page Screenshots

Upload and download app screenshots for an app locale and display target.

## Overview

An `appScreenshots` resource represents a single app screenshot for an app locale and display target. Use this resource to:

- Upload new app screenshots to App Store Connect.

- Download existing screenshots.

To upload screenshots, begin by using the Create an App Screenshot Set endpoint for the locale and display target. To upload screenshots, you must create an asset reservation, then follow the upload operations specified in the response.

## Topics

### Endpoints

List app screenshot sets for a custom product page localization

List the app screenshot sets for a specific custom product page localization.

List All App Screenshots for an App Screenshot Set

List all ordered screenshots in a screenshot set.

Read App Screenshot Information

Get information about an app screenshot and its upload and processing status.

Create an App Screenshot

Add a new screenshot to a screenshot set.

Modify an App Screenshot

Commit an app screenshot after uploading it.

Delete an App Screenshot

Delete an app screenshot that is associated with a screenshot set.

### Objects

object AppScreenshot

The data structure that represent an App Screenshots resource.

object AppScreenshotCreateRequest

The request body you use to create an App Screenshot.

object AppScreenshotUpdateRequest

The request body you use to update an App Screenshot.

object AppScreenshotResponse

A response that contains a single App Screenshots resource.

object AppScreenshotsResponse

A response that contains a list of App Screenshots resources.

object UploadOperation

Upload instructions for assets such as app previews and app screenshots.

## See Also

### Managing Custom Product Page Screenshots

App Custom Product Page Screenshot Sets

Create sets of app screenshots for an app custom product page localization.

