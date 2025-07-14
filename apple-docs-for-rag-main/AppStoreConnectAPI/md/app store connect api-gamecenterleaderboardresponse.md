

- App Store Connect API
-  GameCenterLeaderboardResponse 

Object

# GameCenterLeaderboardResponse

A response that contains a single leaderboard image resource.

App Store Connect API 3.0+

``` source
object GameCenterLeaderboardResponse
```

## Properties

`data`

GameCenterLeaderboard

 (Required) 

`included`

`[*]`

Possible types: GameCenterDetail`, `GameCenterGroup`, `GameCenterLeaderboard`, `GameCenterLeaderboardSet`, `GameCenterLeaderboardLocalization`, `GameCenterLeaderboardRelease

`links`

DocumentLinks

 (Required) 

## See Also

### Objects

object GameCenterLeaderboardUpdateRequest

The request body you use to update a leaderboard.

object GameCenterLeaderboardsResponse

A response that contains multiple leaderboard resources.

object GameCenterLeaderboard

The data structure that represent a leaderboard resource.

object GameCenterLeaderboardCreateRequest

The request body you use to create a leaderboard.

object GameCenterLeaderboardGroupLeaderboardLinkageRequest

The request body you use to attach an individual leaderbaord to a group leaderboard.

object GameCenterLeaderboardGroupLeaderboardLinkageResponse

A response confriming a relationship between a leaderboard and group leaderboard.

