

- App Store Connect API
-  AppCustomProductPageLocalizationsResponse 

Object

# AppCustomProductPageLocalizationsResponse

A response that contains a list of alternative distribution package variant resources.

App Store Connect API 1.7+

``` source
object AppCustomProductPageLocalizationsResponse
```

## Properties

`data`

`[`AppCustomProductPageLocalization`]`

 (Required) 

`included`

`[*]`

Possible types: AppCustomProductPageVersion`, `AppScreenshotSet`, `AppPreviewSet

`links`

PagedDocumentLinks

 (Required) 

`meta`

PagingInformation

## See Also

### Objects

object AppCustomProductPageLocalization

The data structure that represents an app custom product page localization resource.

object AppCustomProductPageLocalizationCreateRequest

The request body you use to create an app custom product page localization.

object AppCustomProductPageLocalizationInlineCreate

The data structure that represents an app custom product page localization inline creates resource.

object AppCustomProductPageLocalizationResponse

A response that contains a single app custom product page resource.

object AppCustomProductPageLocalizationUpdateRequest

The request body you use to update an app custom product page localization.

