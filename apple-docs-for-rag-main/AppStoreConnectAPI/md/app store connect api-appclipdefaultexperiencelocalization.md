

- App Store Connect API
-  AppClipDefaultExperienceLocalization 

Object

# AppClipDefaultExperienceLocalization

The data structure that represents a Default App Clip Experience Localizations resource.

App Store Connect API 1.6+

``` source
object AppClipDefaultExperienceLocalization
```

## Properties

`attributes`

AppClipDefaultExperienceLocalization.Attributes

The attributes that describe the Default App Clip Experience Localizations resource.

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies a Default App Clip Experience Localizations resource.

`links`

ResourceLinks

Navigational links that include the self-link.

`relationships`

AppClipDefaultExperienceLocalization.Relationships

The navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `appClipDefaultExperienceLocalizations`

## Topics

### Objects

object AppClipDefaultExperienceLocalization.Attributes

The attributes that describe a Default App Clip Experience Localizations resource.

object AppClipDefaultExperienceLocalization.Relationships

The relationships of the Default App Clip Experience Localizations resource you included in the request and those on which you can operate.

## See Also

### Objects

object AppClipDefaultExperienceLocalizationResponse

A response that contains a single Default App Clip Experience Localizations resource.

object AppClipDefaultExperienceLocalizationCreateRequest

The request body you use to create a Default App Clip Experience Localization.

object AppClipDefaultExperienceLocalizationUpdateRequest

The request body you use to update a Default App Clip Experiences resource.

object AppClipDefaultExperienceLocalizationsResponse

A response that contains a list of Default App Clip Experience Localizations resources.

