

- App Store Connect API
-  GameCenterAchievementReleasesResponse 

Object

# GameCenterAchievementReleasesResponse

A response that contains a list of achievement release resources.

App Store Connect API 3.0+

``` source
object GameCenterAchievementReleasesResponse
```

## Properties

`data`

`[`GameCenterAchievementRelease`]`

 (Required) 

`included`

`[*]`

Possible types: GameCenterDetail`, `GameCenterAchievement

`links`

PagedDocumentLinks

 (Required) 

`meta`

PagingInformation

## See Also

### Objects

object GameCenterAchievementRelease

The data structure that represent an achievements release resource.

object GameCenterAchievementReleaseCreateRequest

The request body you use to create an achievement release.

object GameCenterAchievementReleaseResponse

A response that contains a single achievement release resource.

