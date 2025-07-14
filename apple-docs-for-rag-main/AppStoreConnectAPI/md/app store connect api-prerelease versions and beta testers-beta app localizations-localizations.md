

- App Store Connect API
- Prerelease Versions and Beta Testers
-  Beta App Localizations 

API Collection

# Beta App Localizations

Beta test information about apps, specific to a locale.

## Overview

A `betaAppLocalization` resource represents one localized set of information about an app that is visible to beta testers. When distributing a prerelease app, the TestFlight app on the beta tester’s device displays information such as descriptions, URLs, and privacy policies. The information can be localized for the languages listed in App Store localizations.

## Topics

### Getting Localization Information

List Beta App Localizations

Find and list beta app localizations for all apps and locales.

Read Beta App Localization Information

Get localized beta app information for a specific app and locale.

Read the App Information of a Beta App Localization

Get the app information associated with a specific beta app localization.

### Creating, Modifying, and Deleting Localizations

Create a Beta App Localization

Create localized descriptive information for an app.

Modify a Beta App Localization

Update the localized information for a specific beta app and locale.

Delete a Beta App Localization

Delete a beta app localization associated with an app.

### Objects

object BetaAppLocalization

The data structure that represents a Beta App Localizations resource.

object BetaAppLocalizationCreateRequest

The request body you use to create a Beta App Localization.

object BetaAppLocalizationResponse

A response that contains a single Beta App Localizations resource.

object BetaAppLocalizationsWithoutIncludesResponse

object BetaAppLocalizationUpdateRequest

The request body you use to update a Beta App Localization.

object BetaAppLocalizationsResponse

A response that contains a list of Beta App Localization resources.

## See Also

### App Resources

Prerelease Versions

Platform-specific versions of your app intended for distribution to beta testers.

Beta License Agreements

Beta license agreements for apps.

