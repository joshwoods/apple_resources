

- App Store Connect API
-  BetaBuildLocalizationsResponse 

Object

# BetaBuildLocalizationsResponse

A response that contains a list of Beta Build Localization resources.

App Store Connect API 1.0+

``` source
object BetaBuildLocalizationsResponse
```

## Properties

`data`

`[`BetaBuildLocalization`]`

 (Required) 

The resource data.

`included`

`[`Build`]`

`links`

PagedDocumentLinks

 (Required) 

Navigational links that include the self-link.

`meta`

PagingInformation

Paging information.

## See Also

### Related Documentation

List Beta Build Localizations

Find and list beta build localizations currently associated with apps.

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

