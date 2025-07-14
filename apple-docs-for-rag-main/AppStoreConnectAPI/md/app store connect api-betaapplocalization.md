

- App Store Connect API
-  BetaAppLocalization 

Object

# BetaAppLocalization

The data structure that represents a Beta App Localizations resource.

App Store Connect API 1.0+

``` source
object BetaAppLocalization
```

## Properties

`attributes`

BetaAppLocalization.Attributes

The resource’s attributes.

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the resource.

`relationships`

BetaAppLocalization.Relationships

Navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `betaAppLocalizations`

`links`

ResourceLinks

Navigational links that include the self-link.

## Topics

### Objects

object BetaAppLocalization.Attributes

Attributes that describe a Beta App Localizations resource.

object BetaAppLocalization.Relationships

The relationships you included in the request and those on which you can operate.

## See Also

### Objects

object BetaAppLocalizationCreateRequest

The request body you use to create a Beta App Localization.

object BetaAppLocalizationResponse

A response that contains a single Beta App Localizations resource.

object BetaAppLocalizationsWithoutIncludesResponse

object BetaAppLocalizationUpdateRequest

The request body you use to update a Beta App Localization.

object BetaAppLocalizationsResponse

A response that contains a list of Beta App Localization resources.

