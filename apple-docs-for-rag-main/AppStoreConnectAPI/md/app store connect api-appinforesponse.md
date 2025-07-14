

- App Store Connect API
-  AppInfoResponse 

Object

# AppInfoResponse

A response that contains a single App Infos resource.

App Store Connect API 1.2+

``` source
object AppInfoResponse
```

## Properties

`data`

AppInfo

 (Required) 

The resource data.

`included`

`[*]`

Possible types: App`, `AgeRatingDeclaration`, `AppInfoLocalization`, `AppCategory

`links`

DocumentLinks

 (Required) 

Navigational links that include the self-link.

## See Also

### Objects

object AppInfo

The data structure that represent an App Infos resource.

object AppInfosResponse

A response that contains a list of App Info resources.

object AppInfoUpdateRequest

The request body you use to update an App Info.

