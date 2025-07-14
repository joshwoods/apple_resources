

- App Store Connect API
-  AppCustomProductPageVersionsResponse 

Object

# AppCustomProductPageVersionsResponse

A response that contains a list of app customer product page version resources.

App Store Connect API 1.7+

``` source
object AppCustomProductPageVersionsResponse
```

## Properties

`data`

`[`AppCustomProductPageVersion`]`

 (Required) 

`included`

`[*]`

Possible types: AppCustomProductPage`, `AppCustomProductPageLocalization

`links`

PagedDocumentLinks

 (Required) 

`meta`

PagingInformation

## See Also

### Objects

object AppCustomProductPageVersion

The data structure that represents an app custom product page version resource.

object AppCustomProductPageVersionCreateRequest

The request body you use to create an app custom product page version.

object AppCustomProductPageVersionInlineCreate

The data structure that represents an app custom product page version inline create resource.

object AppCustomProductPageVersionUpdateRequest

The request body you use to update an app custom product page version.

object AppCustomProductPageVersionResponse

A response that contains a single app custom product page resource.

