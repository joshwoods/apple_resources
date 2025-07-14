

- App Store Connect API
-  GameCenterLeaderboardLocalizationsResponse 

Object

# GameCenterLeaderboardLocalizationsResponse

A response that contains multiple leaderboard localizations resources.

App Store Connect API 3.0+

``` source
object GameCenterLeaderboardLocalizationsResponse
```

## Properties

`data`

`[`GameCenterLeaderboardLocalization`]`

 (Required) 

`included`

`[*]`

Possible types: GameCenterLeaderboard`, `GameCenterLeaderboardImage

`links`

PagedDocumentLinks

 (Required) 

`meta`

PagingInformation

## See Also

### Objects

object GameCenterLeaderboardLocalization

The data structure that represent a leaderboard localization.

object GameCenterLeaderboardLocalizationCreateRequest

The request body you use to create a leaderboard localization.

object GameCenterLeaderboardLocalizationResponse

A response that contains a single leaderboard localization resource.

object GameCenterLeaderboardLocalizationUpdateRequest

The request body you use to update a leaderboard localization.

