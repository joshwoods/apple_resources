

- App Store Connect API
-  GameCenterMatchmakingTeam 

Object

# GameCenterMatchmakingTeam

The data structure that represents a team.

App Store Connect API 3.1+

``` source
object GameCenterMatchmakingTeam
```

## Properties

`attributes`

GameCenterMatchmakingTeam.Attributes

The attributes of the team.

`id`

`string`

 (Required) 

The unique identifier for the team.

`links`

ResourceLinks

The link representations of the object.

`type`

`string`

 (Required) 

The type of resource object.

Value: `gameCenterMatchmakingTeams`

## Topics

### Objects

object GameCenterMatchmakingTeam.Attributes

The attributes of a game-specific team.

## See Also

### Objects

object GameCenterMatchmakingTeamCreateRequest

The request body you use to create a team.

object GameCenterMatchmakingTeamUpdateRequest

The request body you use to modify a team.

object GameCenterMatchmakingTeamResponse

The response body for endpoints that create or modify a team.

object GameCenterMatchmakingTeamsResponse

The response body for endpoints that get multiple teams.

