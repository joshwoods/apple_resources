

- App Store Connect API
- GameCenterLeaderboardCreateRequest
- GameCenterLeaderboardCreateRequest.Data
-  GameCenterLeaderboardCreateRequest.Data.Attributes 

Object

# GameCenterLeaderboardCreateRequest.Data.Attributes

App Store Connect API 3.0+

``` source
object GameCenterLeaderboardCreateRequest.Data.Attributes
```

## Properties

`defaultFormatter`

GameCenterLeaderboardFormatter

 (Required) 

`recurrenceDuration`

`duration`

`recurrenceRule`

`string`

`recurrenceStartDate`

`date-time`

`referenceName`

`string`

 (Required) 

`scoreRangeEnd`

`number`

`scoreRangeStart`

`number`

`scoreSortType`

`string`

 (Required) 

Possible Values: `ASC, DESC`

`submissionType`

`string`

 (Required) 

Possible Values: `BEST_SCORE, MOST_RECENT_SCORE`

`vendorIdentifier`

`string`

 (Required) 

## Mentioned in 

App Store Connect API 3.7 release notes

### Discussion

Use leaderboard formatters to specify the unit of measurement for a Game Center leaderboard. There is a new required attribute `defaultFormatter` when using Create a leaderboard, which gives all your localizations the same formatter. You can also optionally use `formatterOverride` to override a specific leaderboard localization when calling Create a leaderboard localization or Modify a leaderboard localization.

Before App Store Connect API version 3.0, formatters were based on localizations and were required for each localization. Legacy leaderboards created before the new addition of the Game Center APIs don’t have a `defaultFormatter` value; the value is `null`. Any localizations created before the new addition of the Game Center APIs have a `formatterOverride`.

## See Also

### Objects

object GameCenterLeaderboardCreateRequest.Data.Relationships

