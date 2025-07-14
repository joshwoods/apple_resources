

- App Store Connect API
-  GameCenterDetailResponse 

Object

# GameCenterDetailResponse

A response that contains a single Game Center detail resource.

App Store Connect API 3.0+

``` source
object GameCenterDetailResponse
```

## Properties

`data`

GameCenterDetail

 (Required) 

`included`

`[*]`

Possible types: App`, `GameCenterAppVersion`, `GameCenterGroup`, `GameCenterLeaderboard`, `GameCenterLeaderboardSet`, `GameCenterAchievement`, `GameCenterAchievementRelease`, `GameCenterLeaderboardRelease`, `GameCenterLeaderboardSetRelease

`links`

DocumentLinks

 (Required) 

## See Also

### Objects

object GameCenterDetail

The data structure that represents a Game Center detail resource.

object GameCenterDetailCreateRequest

The request body you use to create a Game Center detail.

object GameCenterDetailGameCenterAchievementsLinkagesRequest

The request body you use to create a relationship between a Game Center detail and an achievement.

object GameCenterDetailGameCenterAchievementsLinkagesResponse

A response that confirms a relationship between a Game Center detail and an achievement.

object GameCenterDetailGameCenterLeaderboardSetsLinkagesRequest

The request body you use to create a relationship between a Game Center detail and a leaderboard set.

object GameCenterDetailGameCenterLeaderboardSetsLinkagesResponse

A response that confirms a relationship between a Game Center detail and leaderboard set.

object GameCenterDetailGameCenterLeaderboardsLinkagesRequest

The request body you use to create a relationship between a Game Center detail and a leaderboard.

object GameCenterDetailGameCenterLeaderboardsLinkagesResponse

A response that confirms a relationship between a Game Center detail and a leaderboard.

object GameCenterDetailUpdateRequest

The request body you use to update a Game Center detail.

object GameCenterDetailsResponse

A response that contains a list of Game Center detail resources.

