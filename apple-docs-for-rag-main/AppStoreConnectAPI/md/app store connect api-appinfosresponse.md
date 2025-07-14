

- App Store Connect API
-  AppInfosResponse 

Object

# AppInfosResponse

A response that contains a list of App Info resources.

App Store Connect API 1.2+

``` source
object AppInfosResponse
```

## Properties

`data`

`[`AppInfo`]`

 (Required) 

The resource data.

`included`

`[*]`

Possible types: App`, `AgeRatingDeclaration`, `AppInfoLocalization`, `AppCategory

`links`

PagedDocumentLinks

 (Required) 

Navigational links that include the self-link.

`meta`

PagingInformation

Paging information.

## See Also

### Objects

object AppInfo

The data structure that represent an App Infos resource.

object AppInfoResponse

A response that contains a single App Infos resource.

object AppInfoUpdateRequest

The request body you use to update an App Info.

