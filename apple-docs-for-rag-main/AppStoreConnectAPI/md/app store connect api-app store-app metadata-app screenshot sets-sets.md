

- App Store Connect API
- App Store
- App Metadata
-  App Screenshot Sets 

API Collection

# App Screenshot Sets

Create sets of app screenshots to upload to App Store Connect.

## Overview

An `appScreenshotSets` resource represents a set of screenshots that you intend to upload to App Store Connect. Create an `appScreenshotSets` resource as a container for all screenshots associated with a locale and display target, for example, screenshots for Simplified Chinese on an iPhone with a 6.5” display. Next, upload individual screenshots using the App Screenshots resource.

Important

Some screenshot sizes are required to submit your app for review. For more information, see Screenshot specifications.

## Topics

### Getting Screenshot Sets and Reading Information

Read App Screenshot Set Information

Get an app screenshot set including its display target, language, and the screenshot it contains.

### Creating and Deleting Screenshot Sets

Create an App Screenshot Set

Add a new screenshot set to an App Store version localization for a specific screenshot type and display size.

Delete an App Screenshot Set

Delete an app screenshot set and all of its screenshots.

### Listing and Reordering All Screenshots in a Set

Get All App Screenshot IDs for an App Screenshot Set

Get the ordered screenshot IDs in a screenshot set.

List All App Screenshots for an App Screenshot Set

List all ordered screenshots in a screenshot set.

Replace All App Screenshots for an App Screenshot Set

Change the order of the screenshots in a screenshot set.

### Objects and Data Types

object AppScreenshotSet

The data structure that represent an app screenshot set resource.

object AppScreenshotSetCreateRequest

The request body you use to create an app screenshot set.

object AppScreenshotSetResponse

A response that contains a single app screenshot set resource.

object AppScreenshotSetsResponse

A response that contains a list of app screenshot set resources.

object AppScreenshotSetAppScreenshotsLinkagesRequest

A request body you use to reorder the screenshots in a screenshot set.

object AppScreenshotSetAppScreenshotsLinkagesResponse

A response body that contains a list of related resource IDs.

type ScreenshotDisplayType

A string that represents the display type of an app screenshot.

## See Also

### Managing App Screenshots

App Screenshots

Upload and download app screenshots for an app locale and display target.

