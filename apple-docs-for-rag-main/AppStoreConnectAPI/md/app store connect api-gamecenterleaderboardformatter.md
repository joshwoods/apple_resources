

- App Store Connect API
-  GameCenterLeaderboardFormatter 

Type

# GameCenterLeaderboardFormatter

The values you can select to describe the format of a leaderboard.

App Store Connect API 3.0+

``` source
string GameCenterLeaderboardFormatter
```

## Possible Values 

`INTEGER`  

`DECIMAL_POINT_1_PLACE`  

`DECIMAL_POINT_2_PLACE`  

`DECIMAL_POINT_3_PLACE`  

`ELAPSED_TIME_CENTISECOND`  

`ELAPSED_TIME_MINUTE`  

`ELAPSED_TIME_SECOND`  

`MONEY_POUND_DECIMAL`  

`MONEY_POUND`  

`MONEY_DOLLAR_DECIMAL`  

`MONEY_DOLLAR`  

`MONEY_EURO_DECIMAL`  

`MONEY_EURO`  

`MONEY_FRANC_DECIMAL`  

`MONEY_FRANC`  

`MONEY_KRONER_DECIMAL`  

`MONEY_KRONER`  

`MONEY_YEN`  

## Mentioned in 

App Store Connect API 3.8 release notes

App Store Connect API 3.5 release notes

## Discussion

- PossibleValues

  - INTEGER

  - DECIMAL_POINT_1_PLACE

  - DECIMAL_POINT_2_PLACE

  - DECIMAL_POINT_3_PLACE

  - ELAPSED_TIME_CENTISECOND

  - ELAPSED_TIME_MINUTE

  - ELAPSED_TIME_SECOND

  - MONEY_POUND_DECIMAL

  - MONEY_POUND

  - MONEY_DOLLAR_DECIMAL

  - MONEY_DOLLAR

  - MONEY_EURO_DECIMAL

  - MONEY_EURO

  - MONEY_FRANC_DECIMAL

  - MONEY_FRANC

  - MONEY_KRONER_DECIMAL

  - MONEY_KRONER

  - MONEY_YEN

### Discussion

Leaderboard formatters allow you to specify the unit of measurement for a Game Center leaderboard. There is a new required attribute `defaultFormatter` when using Create a leaderboard which will give all your localizations the same formatter. You can also optionally use `formatterOverride` to override a specific leaderboard localization when calling Create a leaderboard localization or Modify a leaderboard localization.

Before App Store Connect API version 3.0, formatters were based on localizations and were required for each localization. Legacy leaderboards created before the new addition of the Game Center APIs will not have a `defaultFormatter` value, the value would be `null` in this case. Any localizations created before the new addition of the Game Center APIs will always have a `formatterOverride`.

