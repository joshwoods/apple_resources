

- App Store Connect API
-  Create a rule set 

Web Service Endpoint

# Create a rule set

Create a rule set to contain matchmaking rules and teams.

App Store Connect API 3.1+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/gameCenterMatchmakingRuleSets
```

## HTTP Body

GameCenterMatchmakingRuleSetCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

GameCenterMatchmakingRuleSetResponse

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
POST https://api.appstoreconnect.apple.com/v1//gameCenterMatchmakingRuleSets
{
    “data”: {
        “type”: “gameCenterMatchmakingRuleSets”,
        “attributes”: {
            “referenceName”: “com.example.mygame.GameSettingsRuleSet”,
            “ruleLanguageVersion”: 1,
            “minPlayers”: 2,
            “maxPlayers”: 4
        },
        “relationships”: {}
    }
}
```

```
{
    “data”: {
        “type”: “gameCenterMatchmakingRuleSets”,
        “id”: “7353266e-8c6f-4cbe-8f0f-5108332a1146”,
        “attributes”: {
            “referenceName”: “com.example.mygame.GameSettingsRuleSet”,
            “ruleLanguageVersion”: 1,
            “minPlayers”: 2,
            “maxPlayers”: 4
        },
        “relationships”: {
            “teams”: {
                “links”: {
                    “self”: “https://api.appstoreconnect.apple.com/v1/gameCenterMatchmakingRuleSets/7353266e-8c6f-4cbe-8f0f-5108332a1146/relationships/teams”,
                    “related”: “https://api.appstoreconnect.apple.com/v1/gameCenterMatchmakingRuleSets/7353266e-8c6f-4cbe-8f0f-5108332a1146/teams”
                }
            },
            “rules”: {
                “links”: {
                    “self”: “https://api.appstoreconnect.apple.com/v1/gameCenterMatchmakingRuleSets/7353266e-8c6f-4cbe-8f0f-5108332a1146/relationships/rules”,
                    “related”: “https://api.appstoreconnect.apple.com/v1/gameCenterMatchmakingRuleSets/7353266e-8c6f-4cbe-8f0f-5108332a1146/rules”
                }
            },
            “matchmakingQueues”: {
                “links”: {
                    “self”: “https://api.appstoreconnect.apple.com/v1/gameCenterMatchmakingRuleSets/7353266e-8c6f-4cbe-8f0f-5108332a1146/relationships/matchmakingQueues”,
                    “related”: “https://api.appstoreconnect.apple.com/v1/gameCenterMatchmakingRuleSets/7353266e-8c6f-4cbe-8f0f-5108332a1146/matchmakingQueues”
                }
            }
        },
        “links”: {
            “self”: “https://api.appstoreconnect.apple.com/v1/gameCenterMatchmakingRuleSets/7353266e-8c6f-4cbe-8f0f-5108332a1146”
        }
    },
    “links”: {
        “self”: “https://api.appstoreconnect.apple.com/v1/gameCenterMatchmakingRuleSets”
    }
}
```

## See Also

### Creating, modifying, and deleting rule sets

Modify a rule set

Update the attributes of a rule set.

Delete a rule set

Delete a rule set along with its matchmaking rules and teams.

