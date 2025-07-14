

- App Store Connect API
- BetaAppLocalizationUpdateRequest
- BetaAppLocalizationUpdateRequest.Data
-  BetaAppLocalizationUpdateRequest.Data.Attributes 

Object

# BetaAppLocalizationUpdateRequest.Data.Attributes

Attributes whose values you’re changing as part of the update request.

App Store Connect API 1.0+

``` source
object BetaAppLocalizationUpdateRequest.Data.Attributes
```

## Properties

`description`

`string`

A description of your app that highlights features and functionality.

`feedbackEmail`

`string`

An email address to which beta testers can send feedback. Also appears as the reply-to address for TestFlight invitation emails.

`marketingUrl`

`string`

A URL with information about your app. This URL is visible to testers in the TestFlight app

`privacyPolicyUrl`

`string`

A URL that links to your company’s privacy policy. Privacy policies are recommended for all apps that collect user or device-related data or as otherwise required by law.

`tvOsPrivacyPolicy`

`string`

Your company’s privacy policy. Privacy policies are recommended for all apps that collect user or device-related data, or as otherwise required by law.

### Discussion

Important

A description is required for all `betaAppLocalizations` before you can submit to beta app review. After you have added data to the fields for this object, you can change that data, but you cannot remove data.

## See Also

### Related Documentation

Beta App Localizations

Beta test information about apps, specific to a locale.

