

- App Store Connect API
-  GameCenterLeaderboardSetMemberLocalizationsResponse 

Object

# GameCenterLeaderboardSetMemberLocalizationsResponse

A response that contains multiple leaderboard localizations resources.

App Store Connect API 3.0+

``` source
object GameCenterLeaderboardSetMemberLocalizationsResponse
```

## Properties

`data`

`[`GameCenterLeaderboardSetMemberLocalization`]`

 (Required) 

`included`

`[*]`

Possible types: GameCenterLeaderboardSet`, `GameCenterLeaderboard

`links`

PagedDocumentLinks

 (Required) 

`meta`

PagingInformation

## See Also

### Objects

object GameCenterLeaderboardSetMemberLocalization

The data structure that represent a leaderboard set member localization.

object GameCenterLeaderboardSetMemberLocalizationCreateRequest

The request body you use to create a leaderboard set localization.

object GameCenterLeaderboardSetMemberLocalizationResponse

A response that contains a single leaderboard set localization resource.

object GameCenterLeaderboardSetMemberLocalizationUpdateRequest

The request body you use to update a leaderboard localization.

