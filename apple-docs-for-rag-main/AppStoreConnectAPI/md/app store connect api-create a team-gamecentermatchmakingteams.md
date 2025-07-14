

- App Store Connect API
-  Create a team 

Web Service Endpoint

# Create a team

Add a game-specific team to a rule set.

App Store Connect API 3.1+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/gameCenterMatchmakingTeams
```

## HTTP Body

GameCenterMatchmakingTeamCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

GameCenterMatchmakingTeamResponse

`Created`

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## Discussion

### Example Request and Response

- Request
- Response

```
POST https://api.appstoreconnect.apple.com/v1/gameCenterMatchmakingTeams
{
    “data”: {
        “type”: “gameCenterMatchmakingTeams”,
        “attributes”: {
            “minPlayers”: 2,
            “maxPlayers”: 4,
            “referenceName”: “blue”
        },
        “relationships”: {
            “ruleSet”: {
                “data”: {
                    “type”: “gameCenterMatchmakingRuleSets”,
                    “id”: “50d7eed2-8016-441a-a919-db3d863f433c”
                }
            }
        }
    }
}
```

```
{
    “data”: {
        “type”: “gameCenterMatchmakingTeams”,
        “id”: “2a68632b-0129-4c07-8e84-6da57a76499d”,
        “attributes”: {
            “referenceName”: “blue”,
            “minPlayers”: 2,
            “maxPlayers”: 4
        },
        “links”: {
            “self”: “https://api.appstoreconnect.apple.com/v1/gameCenterMatchmakingTeams/2a68632b-0129-4c07-8e84-6da57a76499d”
        }
    },
    “links”: {
        “self”: “https://api.appstoreconnect.apple.com/v1/gameCenterMatchmakingTeams”
    }
}
```

## See Also

### Creating, modifying, and deleting teams

Modify a team

Update a specific team in a rule set.

Delete a team

Delete a game-specific team in a rule set.

