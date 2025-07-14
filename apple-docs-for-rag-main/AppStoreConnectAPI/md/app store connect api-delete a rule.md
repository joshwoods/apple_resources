

- App Store Connect API
-  Delete a rule 

Web Service Endpoint

# Delete a rule

Delete a matchmaking rule in a rule set.

App Store Connect API 3.1+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/gameCenterMatchmakingRules/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

A unique identifier for the rule.

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

### Creating, modifying, and deleting rules

Create a rule

Add a matchmaking rule to a rule set.

Modify a rule

Update a specific matchmaking rule in a rule set.

