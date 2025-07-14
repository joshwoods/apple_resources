

- App Store Connect API
-  GameCenterAppVersionsResponse 

Object

# GameCenterAppVersionsResponse

A response that contains a list of app version resources.

App Store Connect API 3.0+

``` source
object GameCenterAppVersionsResponse
```

## Properties

`data`

`[`GameCenterAppVersion`]`

 (Required) 

`included`

`[*]`

Possible types: GameCenterAppVersion`, `AppStoreVersion

`links`

PagedDocumentLinks

 (Required) 

`meta`

PagingInformation

## See Also

### Objects

object GameCenterAppVersion

The data structure that represents a Game Center app version resource.

object GameCenterAppVersionCompatibilityVersionsLinkagesRequest

The request body you use to create a relationship between an app version and a compatibility version.

object GameCenterAppVersionCompatibilityVersionsLinkagesResponse

A response that confirms a relationship between an app version and a compatilibty version.

object GameCenterAppVersionCreateRequest

The request body you use to create an app version.

object GameCenterAppVersionResponse

A response that contains a single app version resource.

object GameCenterAppVersionUpdateRequest

The request body you use to update an app version.

