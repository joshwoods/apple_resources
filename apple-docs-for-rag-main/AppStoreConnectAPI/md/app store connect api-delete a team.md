

- App Store Connect API
-  Delete a team 

Web Service Endpoint

# Delete a team

Delete a game-specific team in a rule set.

App Store Connect API 3.1+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/gameCenterMatchmakingTeams/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The unique identifier for the team.

## Response Codes

` 204 ``No Content`

`No Content`

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

## See Also

### Creating, modifying, and deleting teams

Create a team

Add a game-specific team to a rule set.

Modify a team

Update a specific team in a rule set.

