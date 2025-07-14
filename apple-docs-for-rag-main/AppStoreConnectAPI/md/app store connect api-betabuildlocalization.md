

- App Store Connect API
-  BetaBuildLocalization 

Object

# BetaBuildLocalization

The data structure that represents a Beta Build Localizations resource.

App Store Connect API 1.0+

``` source
object BetaBuildLocalization
```

## Properties

`attributes`

BetaBuildLocalization.Attributes

The resource’s attributes.

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the resource.

`relationships`

BetaBuildLocalization.Relationships

Navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `betaBuildLocalizations`

`links`

ResourceLinks

Navigational links that include the self-link.

## Topics

### Objects

object BetaBuildLocalization.Attributes

Attributes that describe a Beta Build Localizations resource.

object BetaBuildLocalization.Relationships

The relationships you included in the request and those on which you can operate.

## See Also

### Objects

object BetaBuildLocalizationResponse

A response that contains a single Beta Build Localizations resource.

object BetaBuildLocalizationsWithoutIncludesResponse

object BetaBuildLocalizationCreateRequest

The request body you use to create a Beta Build Localization.

object BetaBuildLocalizationUpdateRequest

The request body you use to update a Beta Build Localization.

object BetaBuildLocalizationsResponse

A response that contains a list of Beta Build Localization resources.

