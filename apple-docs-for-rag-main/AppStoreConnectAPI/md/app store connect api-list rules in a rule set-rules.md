

- App Store Connect API
-  List rules in a rule set 

Web Service Endpoint

# List rules in a rule set

Get information about the rules in a rule set.

App Store Connect API 3.1+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/gameCenterMatchmakingRuleSets/{id}/rules
```

## Path Parameters

`id`

`string`

 (Required) 

The unique identifier for the rule set.

## Query Parameters

`fields[gameCenterMatchmakingRules]`

`[string]`

The fields of the rules to include in the response.

Possible Values: `referenceName, description, type, expression, weight`

`limit`

`integer`

The maximum number of rules to fetch.

Maximum: `200`

## Response Codes

` 200 ``OK`

GameCenterMatchmakingRulesResponse

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

## See Also

### Reading rule set information

List all rule sets

Get information about all rule sets and their associated objects.

Read rule set information

Get information about a specific rule set and its related objects.

List queues in a rule set

Get information about queues that belong to a rule set.

List teams in a rule set

Get information about the teams in a rule set.

