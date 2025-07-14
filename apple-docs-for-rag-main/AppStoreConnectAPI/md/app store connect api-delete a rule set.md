

- App Store Connect API
-  Delete a rule set 

Web Service Endpoint

# Delete a rule set

Delete a rule set along with its matchmaking rules and teams.

App Store Connect API 3.1+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/gameCenterMatchmakingRuleSets/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

A unique identifier for the rule set.

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

### Creating, modifying, and deleting rule sets

Create a rule set

Create a rule set to contain matchmaking rules and teams.

Modify a rule set

Update the attributes of a rule set.

