

- App Store Connect API
- App Store
- App Metadata
-  App Info Localizations 

API Collection

# App Info Localizations

Manage the app metadata that is localized and appears on the App Store.

## Overview

`appInfoLocalizations` represent your app’s localized metadata that is displayed in the App Store. You can create, read, update, and remove the localized metadata. It includes the following attributes for each localization:

- Locale

- Name

- Subtitle

- Privacy policy URL

- Privacy policy text (for tvOS apps)

You can update localized metadata when your app is in an editable state. For more information about the metadata, see Localize App Store information. For a list of supported languages, see App Store localizations.

Note

The languages you add to an `appInfoLocalizations` resource only affect your app’s metadata. To add languages to your app’s binary, see What is localization.

## Topics

### Essentials

Managing metadata in your app by using locale shortcodes

Optimize your app’s user experience by adding localized metadata with App Store Connect API.

### Reading App Localization Information

List All App Info Localizations for an App Info

Get a list of localized, app-level information for an app.

Read App Info Localization Information

Read localized app-level information.

### Creating, Modifying, and Deleting Localized App Information

Create an App Info Localization

Add app-level localized information for a new locale.

Modify an App Info Localization

Modify localized app-level information for a particular language.

Delete an App Info Localization

Delete an app information localization that is associated with an app.

### Objects

object AppInfoLocalization

The data structure that represent an App Info Localizations resource.

object AppInfoLocalizationCreateRequest

The request body you use to create an App Info Localization.

object AppInfoLocalizationResponse

A response that contains a single App Info Localizations resource.

object AppInfoLocalizationUpdateRequest

The request body you use to update an App Info Localization.

object AppInfoLocalizationsResponse

A response that contains a list of AppInfoLocalizations resources.

## See Also

### Managing App Information and Versions

App Infos

Manage or read the app metadata that applies across all versions of your app.

App Store Versions

Manage versions of your app that are available in App Store.

App Store Version Localizations

Create and maintain version-specific App Store metadata that’s localized.

Routing App Coverages

Manage geographic coverage files for apps that use location to provide routing information.

