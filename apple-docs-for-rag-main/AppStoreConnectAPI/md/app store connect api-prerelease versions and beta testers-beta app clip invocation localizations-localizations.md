

- App Store Connect API
- Prerelease Versions and Beta Testers
-  Beta App Clip Invocation Localizations 

API Collection

# Beta App Clip Invocation Localizations

Manage beta test information for an App Clip and its invocation, specific to a locale.

## Overview

The `betaAppClipInvocationLocalizations` resource represents the localization information of an App Clip you distribute to testers that’s specific to a locale. Use this resource to set the text that appears in the App Clips section of a build in the TestFlight app.

For more information on testing App Clip invocations, see Testing the launch experience of your App Clip.

## Topics

### Managing Localizations for Invocations of Beta App Clips

Create Localized Metadata for a Beta App Clip Invocation

Provide localized metadata for an App Clip experience you make available to testers.

Modify Localized Metadata of an App Clip Invocation for Testers

Change the metadata for an App Clip you make available to testers in the TestFlight app.

Delete a Beta App Clip Invocation Localization

Delete localized metadata you configured for an App Clip that testers launch using the TestFlight app.

### Objects

object BetaAppClipInvocationLocalization

The data structure that represents a Beta App Clip Invocation Localizations resource.

object BetaAppClipInvocationLocalizationCreateRequest

The request body you use to create a Beta App Clip Localization.

object BetaAppClipInvocationLocalizationUpdateRequest

The request body you use to update localized text that appears on the App Clip card for testers.

object BetaAppClipInvocationLocalizationResponse

A response that contains a single Beta App Clip Invocation Localizations resource.

## See Also

### App Clip Resources

Beta App Clip Invocations

Manage App Clip experiences for testers in TestFlight.

