

- App Store Connect API
- App Store
- App Metadata
-  App Infos 

API Collection

# App Infos

Manage or read the app metadata that applies across all versions of your app.

## Overview

`appInfos` represents your app’s metadata that applies across all versions of your app. You can update your app’s App Store category, subcategory, and secondary category through the `appInfos` resource. You can also find your app’s status, which tells you if the app metadata is editable. For more information, see App and submission statuses.

Other attributes in `appInfos` are read-only. Their values are derived from other resources. For example, your app’s `appStoreAgeRating` value results from the answers you provide to the questions in `ageRatingDeclarations`.

For more information about the metadata in the `appInfos` resource, see App and submission statuses.

## Topics

### Reading App Information

Read App Info Information

Read App Store information including your App Store state, age ratings, Brazil age rating, and kids’ age band.

List All App Infos for an App

Get information about an app that is currently live on App Store, or that goes live with the next version.

List All App Info Localizations for an App Info

Get a list of localized, app-level information for an app.

### Modifying App Information

Modify an App Info

Update the App Store categories and sub-categories for your app.

### Reading Category Information

App Categories and Subcategories

Read the category and subcategory information of an App Info.

### Reading Localization Information

List All App Info Localizations for an App Info

Get a list of localized, app-level information for an app.

### Reading Age Rating Information

Read age rating declaration

Get the age rating declaration for the app info.

### Objects

object AppInfo

The data structure that represent an App Infos resource.

object AppInfoResponse

A response that contains a single App Infos resource.

object AppInfosResponse

A response that contains a list of App Info resources.

object AppInfoUpdateRequest

The request body you use to update an App Info.

## See Also

### Managing App Information and Versions

App Info Localizations

Manage the app metadata that is localized and appears on the App Store.

App Store Versions

Manage versions of your app that are available in App Store.

App Store Version Localizations

Create and maintain version-specific App Store metadata that’s localized.

Routing App Coverages

Manage geographic coverage files for apps that use location to provide routing information.

