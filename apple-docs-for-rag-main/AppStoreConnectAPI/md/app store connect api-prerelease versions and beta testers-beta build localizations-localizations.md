

- App Store Connect API
- Prerelease Versions and Beta Testers
-  Beta Build Localizations 

API Collection

# Beta Build Localizations

Beta test information about builds, specific to a locale.

## Overview

A `betaBuildLocalizations` resource represents the localized content that appears in the “What’s New” text in TestFlight. You should change this text for every build.

## Topics

### Getting Build Information

List Beta Build Localizations

Find and list beta build localizations currently associated with apps.

Read Beta Build Localization Information

Get a specific beta build localization resource.

Read the Build Information of a Beta Build Localization

Get the build information for a specific beta build localization.

### Creating, Modifying, and Deleting Beta Build Localizations

Create a Beta Build Localization

Create localized What’s New text for a build.

Modify a Beta Build Localization

Update the localized What’s New text for a specific beta build and locale.

Delete a Beta Build Localization

Delete a specific beta build localization associated with a build.

### Objects

object BetaBuildLocalization

The data structure that represents a Beta Build Localizations resource.

object BetaBuildLocalizationResponse

A response that contains a single Beta Build Localizations resource.

object BetaBuildLocalizationsWithoutIncludesResponse

object BetaBuildLocalizationCreateRequest

The request body you use to create a Beta Build Localization.

object BetaBuildLocalizationUpdateRequest

The request body you use to update a Beta Build Localization.

object BetaBuildLocalizationsResponse

A response that contains a list of Beta Build Localization resources.

## See Also

### Build Resources

Builds

Manage builds for testers and submit builds for review.

Build Beta Details

TestFlight-specific information about beta builds.

Build Beta Notifications

Requests to send notifications to all assigned testers that builds are ready for testing.

