

- App Store Connect API
-  Modify a team 

Web Service Endpoint

# Modify a team

Update a specific team in a rule set.

App Store Connect API 3.1+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/gameCenterMatchmakingTeams/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The unique identifier for the team.

## HTTP Body

GameCenterMatchmakingTeamUpdateRequest

Content-Type: application/json

## Response Codes

` 200 ``OK`

GameCenterMatchmakingTeamResponse

`OK`

Content-Type: application/json

` 400 ``Bad Request`

ErrorResponse

`Bad Request`

Content-Type: application/json

` 401 ``Unauthorized`

ErrorResponse

`Unauthorized`

Content-Type: application/json

` 403 ``Forbidden`

ErrorResponse

`Forbidden`

Content-Type: application/json

` 404 ``Not Found`

ErrorResponse

`Not Found`

Content-Type: application/json

` 409 ``Conflict`

ErrorResponse

`Conflict`

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## See Also

### Creating, modifying, and deleting teams

Create a team

Add a game-specific team to a rule set.

Delete a team

Delete a game-specific team in a rule set.

