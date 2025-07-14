

- App Store Connect API
-  Modify a rule set 

Web Service Endpoint

# Modify a rule set

Update the attributes of a rule set.

App Store Connect API 3.1+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/gameCenterMatchmakingRuleSets/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

A unique identifier for the rule set.

## HTTP Body

GameCenterMatchmakingRuleSetUpdateRequest

Content-Type: application/json

## Response Codes

` 200 ``OK`

GameCenterMatchmakingRuleSetResponse

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

### Creating, modifying, and deleting rule sets

Create a rule set

Create a rule set to contain matchmaking rules and teams.

Delete a rule set

Delete a rule set along with its matchmaking rules and teams.

