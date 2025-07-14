

- App Store Connect API
-  GameCenterAchievementsResponse 

Object

# GameCenterAchievementsResponse

A response that contains a list of Game Center achievement resources.

App Store Connect API 3.0+

``` source
object GameCenterAchievementsResponse
```

## Properties

`data`

`[`GameCenterAchievement`]`

 (Required) 

`included`

`[*]`

Possible types: GameCenterDetail`, `GameCenterGroup`, `GameCenterAchievement`, `GameCenterAchievementLocalization`, `GameCenterAchievementRelease

`links`

PagedDocumentLinks

 (Required) 

`meta`

PagingInformation

## See Also

### Objects

object GameCenterAchievement

The data structure that represents a Game Center achievement resource.

object GameCenterAchievementCreateRequest

A request body you use to create a Game Center achievement.

object GameCenterAchievementGroupAchievementLinkageRequest

The request body you use to attach an achievement to an achievement group.

object GameCenterAchievementGroupAchievementLinkageResponse

A response body that contains the ID of a single related resource.

object GameCenterAchievementResponse

A response that contains a single Game Center achievement resource.

object GameCenterAchievementUpdateRequest

The request body you use to update a Game Center achievement.

