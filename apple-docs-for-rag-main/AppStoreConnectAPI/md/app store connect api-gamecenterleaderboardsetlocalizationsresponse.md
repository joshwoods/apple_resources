

- App Store Connect API
-  GameCenterLeaderboardSetLocalizationsResponse 

Object

# GameCenterLeaderboardSetLocalizationsResponse

A response that contains multiple leaderboard localizations resources.

App Store Connect API 3.0+

``` source
object GameCenterLeaderboardSetLocalizationsResponse
```

## Properties

`data`

`[`GameCenterLeaderboardSetLocalization`]`

 (Required) 

`included`

`[*]`

Possible types: GameCenterLeaderboardSet`, `GameCenterLeaderboardSetImage

`links`

PagedDocumentLinks

 (Required) 

`meta`

PagingInformation

## See Also

### Objects

object GameCenterLeaderboardSetLocalization

The data structure that represent a leaderboard set localization.

object GameCenterLeaderboardSetLocalizationCreateRequest

The request body you use to create a leaderboard set localization.

object GameCenterLeaderboardSetLocalizationResponse

A response that contains a single leaderboard set localization resource.

object GameCenterLeaderboardSetLocalizationUpdateRequest

The request body you use to update a leaderboard localization.

