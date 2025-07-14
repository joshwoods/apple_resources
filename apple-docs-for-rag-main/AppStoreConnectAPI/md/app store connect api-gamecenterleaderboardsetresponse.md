

- App Store Connect API
-  GameCenterLeaderboardSetResponse 

Object

# GameCenterLeaderboardSetResponse

A response that contains a single leaderboard set resource.

App Store Connect API 3.0+

``` source
object GameCenterLeaderboardSetResponse
```

## Properties

`data`

GameCenterLeaderboardSet

 (Required) 

`included`

`[*]`

Possible types: GameCenterDetail`, `GameCenterGroup`, `GameCenterLeaderboardSet`, `GameCenterLeaderboardSetLocalization`, `GameCenterLeaderboard`, `GameCenterLeaderboardSetRelease

`links`

DocumentLinks

 (Required) 

## See Also

### Objects

object GameCenterLeaderboardSet

The data structure that represent a leaderboard set resource.

object GameCenterLeaderboardSetCreateRequest

The request body you use to create a leaderboard set.

object GameCenterLeaderboardSetGameCenterLeaderboardsLinkagesRequest

The request body you use to create a relationship between a leaderboard set and a leaderboard.

object GameCenterLeaderboardSetGameCenterLeaderboardsLinkagesResponse

A response that confirms a relationship between a leaderboard set and a leaderboard.

object GameCenterLeaderboardSetGroupLeaderboardSetLinkageRequest

The request body you use to create a relationship between a leaderboard set and a group leaderboard set.

object GameCenterLeaderboardSetGroupLeaderboardSetLinkageResponse

A response that confirms a relationship between a leaderboard set and a group leaderboard set.

object GameCenterLeaderboardSetUpdateRequest

The request body you use to update a leaderboard set.

object GameCenterLeaderboardSetsResponse

A response that contains multiple leaderboard set resources.

