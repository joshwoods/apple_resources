

- App Store Connect API
-  BetaAppLocalizationsResponse 

Object

# BetaAppLocalizationsResponse

A response that contains a list of Beta App Localization resources.

App Store Connect API 1.0+

``` source
object BetaAppLocalizationsResponse
```

## Properties

`data`

`[`BetaAppLocalization`]`

 (Required) 

The resource data.

`links`

PagedDocumentLinks

 (Required) 

Navigational links that include the self-link.

`meta`

PagingInformation

Paging information.

`included`

`[`App`]`

## See Also

### Related Documentation

List Beta App Localizations

Find and list beta app localizations for all apps and locales.

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

