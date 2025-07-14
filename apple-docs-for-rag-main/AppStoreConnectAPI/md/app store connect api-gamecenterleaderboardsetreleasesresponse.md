

- App Store Connect API
-  GameCenterLeaderboardSetReleasesResponse 

Object

# GameCenterLeaderboardSetReleasesResponse

A response that contains multiple leaderboard set release resource.

App Store Connect API 3.0+

``` source
object GameCenterLeaderboardSetReleasesResponse
```

## Properties

`data`

`[`GameCenterLeaderboardSetRelease`]`

 (Required) 

`included`

`[*]`

Possible types: GameCenterDetail`, `GameCenterLeaderboardSet

`links`

PagedDocumentLinks

 (Required) 

`meta`

PagingInformation

## See Also

### Objects

object GameCenterLeaderboardSetRelease

The data structure that represent a leaderboard set release.

object GameCenterLeaderboardSetReleaseCreateRequest

The request body you use to create a leaderboard set release.

object GameCenterLeaderboardSetReleaseResponse

A response that contains a single leaderboard set release resource.

