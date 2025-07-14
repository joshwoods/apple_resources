

- App Store Connect API
-  GameCenterAchievementResponse 

Object

# GameCenterAchievementResponse

A response that contains a single Game Center achievement resource.

App Store Connect API 3.0+

``` source
object GameCenterAchievementResponse
```

## Properties

`data`

GameCenterAchievement

 (Required) 

`included`

`[*]`

Possible types: GameCenterDetail`, `GameCenterGroup`, `GameCenterAchievement`, `GameCenterAchievementLocalization`, `GameCenterAchievementRelease

`links`

DocumentLinks

 (Required) 

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

object GameCenterAchievementUpdateRequest

The request body you use to update a Game Center achievement.

object GameCenterAchievementsResponse

A response that contains a list of Game Center achievement resources.

