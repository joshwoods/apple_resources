

- App Store Connect API
- App Store
- App Metadata
-  App Store Version Localizations 

API Collection

# App Store Version Localizations

Create and maintain version-specific App Store metadata that’s localized.

## Overview

Use `appStoreVersionLocalizations` to create and maintain your App Store metadata in different languages. This resource includes the following attributes:

- Locale

- Description

- Keywords

- Marketing URL

- Promotional Text

- Support URL

- What’s New Text

You can update the Promotional Text for your version at any time. Update other attributes when your app is in an editable state. For information about required, localized, and editable metadata, see Required, localized, and editable properties.

## Topics

### Getting Version Localizations

List All App Store Version Localizations for an App Store Version

Get a list of localized, version-level information about an app, for all locales.

Read App Store Version Localization Information

Read localized version-level information.

### Creating, Modifying, and Deleting Version Localizations

Create an App Store Version Localization

Add localized version-level information for a new locale.

Modify an App Store Version Localization

Modify localized version-level information for a particular language.

Delete an App Store Version Localization

Delete a language from your version metadata.

### Getting Information from a Localization

List All App Screenshot Sets for an App Store Version Localization

List all screenshot sets for a specific localization.

List All App Preview Sets for an App Store Version Localization

List all app preview sets for a specific localization.

### Objects

object AppStoreVersionLocalization

The data structure that represent an App Store Version Localizations resource.

object AppStoreVersionLocalizationCreateRequest

The request body you use to create an App Store Version Localization.

object AppStoreVersionLocalizationResponse

A response that contains a single App Store Version Localizations resource.

object AppStoreVersionLocalizationsResponse

A response that contains a list of App Store Version Localization resources.

object AppStoreVersionLocalizationUpdateRequest

The request body you use to update an App Store Version Localization

## See Also

### Managing App Information and Versions

App Infos

Manage or read the app metadata that applies across all versions of your app.

App Info Localizations

Manage the app metadata that is localized and appears on the App Store.

App Store Versions

Manage versions of your app that are available in App Store.

Routing App Coverages

Manage geographic coverage files for apps that use location to provide routing information.

