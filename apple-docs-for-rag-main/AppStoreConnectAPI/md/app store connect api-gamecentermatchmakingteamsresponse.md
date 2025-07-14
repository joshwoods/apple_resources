

- App Store Connect API
-  GameCenterMatchmakingTeamsResponse 

Object

# GameCenterMatchmakingTeamsResponse

The response body for endpoints that get multiple teams.

App Store Connect API 3.1+

``` source
object GameCenterMatchmakingTeamsResponse
```

## Properties

`data`

`[`GameCenterMatchmakingTeam`]`

 (Required) 

The teams that the endpoint fetches.

`links`

PagedDocumentLinks

 (Required) 

The link representations of the object.

`meta`

PagingInformation

## See Also

### Objects

object GameCenterMatchmakingTeamCreateRequest

The request body you use to create a team.

object GameCenterMatchmakingTeamUpdateRequest

The request body you use to modify a team.

object GameCenterMatchmakingTeamResponse

The response body for endpoints that create or modify a team.

object GameCenterMatchmakingTeam

The data structure that represents a team.

