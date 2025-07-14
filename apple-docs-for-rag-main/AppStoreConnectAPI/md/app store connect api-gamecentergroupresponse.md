

- App Store Connect API
-  GameCenterGroupResponse 

Object

# GameCenterGroupResponse

A response that contains a single group resource.

App Store Connect API 3.0+

``` source
object GameCenterGroupResponse
```

## Properties

`data`

GameCenterGroup

 (Required) 

`included`

`[*]`

Possible types: GameCenterDetail`, `GameCenterLeaderboard`, `GameCenterLeaderboardSet`, `GameCenterAchievement

`links`

DocumentLinks

 (Required) 

## See Also

### Objects

object GameCenterGroup

The data structure that represents a group resource.

object GameCenterGroupCreateRequest

The request body you use to create a group.

object GameCenterGroupGameCenterAchievementsLinkagesRequest

The request body you use to create a relationship between a group and an achievement.

object GameCenterGroupGameCenterAchievementsLinkagesResponse

A response that confirms a relationship between a group and an achievement.

object GameCenterGroupGameCenterLeaderboardSetsLinkagesRequest

The request body you use to create a relationship between a group and a leaderboard set.

object GameCenterGroupGameCenterLeaderboardSetsLinkagesResponse

A response that confirms a relationship between a group and leaderboard set.

object GameCenterGroupGameCenterLeaderboardsLinkagesRequest

The request body you use to create a relationship between a group and a leaderboard.

object GameCenterGroupGameCenterLeaderboardsLinkagesResponse

A response that confirms a relationship between a group and a leaderboard.

object GameCenterGroupUpdateRequest

The request body you use to update a group.

object GameCenterGroupsResponse

A response that contains one or more groups.

