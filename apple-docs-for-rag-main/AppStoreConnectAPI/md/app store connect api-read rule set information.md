

- App Store Connect API
-  Read rule set information 

Web Service Endpoint

# Read rule set information

Get information about a specific rule set and its related objects.

App Store Connect API 3.1+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/gameCenterMatchmakingRuleSets/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The unique identifier for the rule set.

## Query Parameters

`fields[gameCenterMatchmakingQueues]`

`[string]`

The fields of the queues to include in the response.

Possible Values: `referenceName, classicMatchmakingBundleIds, ruleSet, experimentRuleSet`

`fields[gameCenterMatchmakingRuleSets]`

`[string]`

The fields of the rule set to include in the response.

Possible Values: `referenceName, ruleLanguageVersion, minPlayers, maxPlayers, teams, rules, matchmakingQueues`

`fields[gameCenterMatchmakingRules]`

`[string]`

The fields of the rules to include in the response.

Possible Values: `referenceName, description, type, expression, weight`

`fields[gameCenterMatchmakingTeams]`

`[string]`

The fields of the teams to include in the response.

Possible Values: `referenceName, minPlayers, maxPlayers`

`include`

`[string]`

The relationships to include in the response.

Possible Values: `teams, rules, matchmakingQueues`

`limit[matchmakingQueues]`

`integer`

The maximum number of queues to fetch.

Maximum: `50`

`limit[rules]`

`integer`

The maximum number of rules to fetch.

Maximum: `50`

`limit[teams]`

`integer`

The maximum number of teams to fetch.

Maximum: `50`

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

## See Also

### Reading rule set information

List all rule sets

Get information about all rule sets and their associated objects.

List queues in a rule set

Get information about queues that belong to a rule set.

List rules in a rule set

Get information about the rules in a rule set.

List teams in a rule set

Get information about the teams in a rule set.

