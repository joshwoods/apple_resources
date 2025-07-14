

- App Store Connect API
- BetaAppLocalizationCreateRequest
- BetaAppLocalizationCreateRequest.Data
-  BetaAppLocalizationCreateRequest.Data.Attributes 

Object

# BetaAppLocalizationCreateRequest.Data.Attributes

Attributes that you set that describe the new resource.

App Store Connect API 1.0+

``` source
object BetaAppLocalizationCreateRequest.Data.Attributes
```

## Properties

`description`

`string`

A description of your app that highlights features and functionality.

`feedbackEmail`

`string`

An email address to which beta testers can send feedback. Also appears as the reply-to address for TestFlight invitation emails.

`locale`

`string`

 (Required) 

The specified locale. To learn more, see Managing metadata in your app by using locale shortcodes.

`marketingUrl`

`string`

A URL with information about your app. This URL is visible to testers in the TestFlight app.

`privacyPolicyUrl`

`string`

A URL that links to your company’s privacy policy. Privacy policies are recommended for all apps that collect user or device-related data or as otherwise required by law.

`tvOsPrivacyPolicy`

`string`

Your company’s privacy policy. Privacy policies are recommended for all apps that collect user or device-related data, or as otherwise required by law.

## See Also

### Related Documentation

Beta App Localizations

Beta test information about apps, specific to a locale.

### Objects

object BetaAppLocalizationCreateRequest.Data.Relationships

The relationships to other resources that you can set with this request.

