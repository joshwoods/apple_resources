

- App Store Connect API
- GameCenterLeaderboardLocalizationUpdateRequest
- GameCenterLeaderboardLocalizationUpdateRequest.Data
-  GameCenterLeaderboardLocalizationUpdateRequest.Data.Attributes 

Object

# GameCenterLeaderboardLocalizationUpdateRequest.Data.Attributes

App Store Connect API 3.0+

``` source
object GameCenterLeaderboardLocalizationUpdateRequest.Data.Attributes
```

## Properties

`formatterOverride`

GameCenterLeaderboardFormatter

`formatterSuffix`

`string`

`formatterSuffixSingular`

`string`

`name`

`string`

### Discussion

Use leaderboard formatters to specify the unit of measurement for a Game Center leaderboard. There is a new required attribute `defaultFormatter` when you use Create a leaderboard, which gives all your localizations the same formatter. You can also optionally use `formatterOverride` to override a specific leaderboard localization when calling Create a leaderboard localization or Modify a leaderboard localization.

Before App Store Connect API version 3.0, formatters were based on localizations and were required for each localization. Legacy leaderboards created before the new addition of the Game Center APIs will not have a `defaultFormatter` value, the value would be `null` in this case. Any localizations created before the new addition of the Game Center APIs will always have a `formatterOverride`.

