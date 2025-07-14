

- App Store Connect API
- GameCenterMatchmakingRuleSetCreateRequest
- GameCenterMatchmakingRuleSetCreateRequest.Data
-  GameCenterMatchmakingRuleSetCreateRequest.Data.Attributes 

Object

# GameCenterMatchmakingRuleSetCreateRequest.Data.Attributes

The attributes for a rule set that you create.

App Store Connect API 3.1+

``` source
object GameCenterMatchmakingRuleSetCreateRequest.Data.Attributes
```

## Properties

`maxPlayers`

`integer`

 (Required) 

The maximum number of players who can join the matches that Game Center finds using these rules.

`minPlayers`

`integer`

 (Required) 

The minimum number of players who can join the matches that Game Center finds using these rules.

`referenceName`

`string`

 (Required) 

A name for the rule set that’s unique within the scope of your development team.

`ruleLanguageVersion`

`integer`

 (Required) 

The version of the expression language that all the rules in this rule set use. The only possible value is `1`.

## Discussion

The `minPlayers` and `maxPlayers` attributes constrain the range of players in the match requests. If you don’t set the `GKMatchRequest.`minPlayers and `GKMatchRequest.`maxPlayers properties in your code, the properties default to the rule set `minPlayers` and `maxPlayers` attributes. If you set the GKMatchRequest properties, use values that are in the rule set range.

For example, if the match request range is `[2, 4]` and the rule set range is `[2,8]`, Game Center finds players within the `[2, 4]` match request range. However, if the match request range is `[2, 8]` and the rule set range is `[3, 4]`, Game Center ignores the match request properties and finds players within the `[3, 4]` rule set range. If the match request range is `[8, 8]` and the rule set range is `[2, 4]` (outside of the rule set range), Game Center never finds players for that request.

