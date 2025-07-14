

- App Store Connect API
-  GameCenterLeaderboardReleasesResponse 

Object

# GameCenterLeaderboardReleasesResponse

A response that contains multiple leaderboard release resource.

App Store Connect API 3.0+

``` source
object GameCenterLeaderboardReleasesResponse
```

## Properties

`data`

`[`GameCenterLeaderboardRelease`]`

 (Required) 

`included`

`[*]`

Possible types: GameCenterDetail`, `GameCenterLeaderboard

`links`

PagedDocumentLinks

 (Required) 

`meta`

PagingInformation

## See Also

### Objects

object GameCenterLeaderboardRelease

The data structure that represents a leaderboard release.

object GameCenterLeaderboardReleaseCreateRequest

The request body you use to create a leaderboard release.

object GameCenterLeaderboardReleaseResponse

A response that contains a single leaderboard release resource.

