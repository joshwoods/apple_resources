

- App Store Connect API
-  Create a rule 

Web Service Endpoint

# Create a rule

Add a matchmaking rule to a rule set.

App Store Connect API 3.1+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/gameCenterMatchmakingRules
```

## HTTP Body

GameCenterMatchmakingRuleCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

GameCenterMatchmakingRuleResponse

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
POST https://api.appstoreconnect.apple.com/v1/gameCenterMatchmakingRules
{
    “data”: {
        “type”: “gameCenterMatchmakingRules”,
        “attributes”: {
            “type”: “COMPATIBLE”,
            “description”: “Check whether the players use the same game settings.”,
            “referenceName”: “SameTheme”,
            “expression”: “requests[0].properties.theme == requests[1].properties.theme”
        },
        “relationships”: {
            “ruleSet”: {
                “data”: {
                    “type”: “gameCenterMatchmakingRuleSets”,
                    “id”: “7353266e-8c6f-4cbe-8f0f-5108332a1146”
                }
            }
        }
    }
}
```

```
{
    “data”: {
        “type”: “gameCenterMatchmakingRules”,
        “id”: “2fd4bb73-3cca-46ca-aced-395c54ab11bc”,
        “attributes”: {
            “referenceName”: “SameTheme”,
            “description”: “Check whether the players use the same game settings.”,
            “type”: “COMPATIBLE”,
            “expression”: “requests[0].properties.theme == requests[1].properties.theme”,
            “weight”: null
        },
        “links”: {
            “self”: “https://api.appstoreconnect.apple.com/v1/gameCenterMatchmakingRules/2fd4bb73-3cca-46ca-aced-395c54ab11bc”
        }
    },
    “links”: {
        “self”: “https://api.appstoreconnect.apple.com/v1/gameCenterMatchmakingRules”
    }
}
```

## See Also

### Creating, modifying, and deleting rules

Modify a rule

Update a specific matchmaking rule in a rule set.

Delete a rule

Delete a matchmaking rule in a rule set.

