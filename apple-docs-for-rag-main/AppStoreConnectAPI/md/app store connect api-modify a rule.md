

- App Store Connect API
-  Modify a rule 

Web Service Endpoint

# Modify a rule

Update a specific matchmaking rule in a rule set.

App Store Connect API 3.1+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/gameCenterMatchmakingRules/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The unique identifier for the rule.

## HTTP Body

GameCenterMatchmakingRuleUpdateRequest

Content-Type: application/json

## Response Codes

` 200 ``OK`

GameCenterMatchmakingRuleResponse

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

### Creating, modifying, and deleting rules

Create a rule

Add a matchmaking rule to a rule set.

Delete a rule

Delete a matchmaking rule in a rule set.

