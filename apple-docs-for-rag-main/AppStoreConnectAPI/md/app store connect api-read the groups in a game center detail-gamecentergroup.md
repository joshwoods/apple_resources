

- App Store Connect API
-  Read the groups in a Game Center detail 

Web Service Endpoint

# Read the groups in a Game Center detail

Get a list of groups in a Game Center detail.

App Store Connect API 3.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/gameCenterDetails/{id}/gameCenterGroup
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[gameCenterAchievements]`

`[string]`

Possible Values: `referenceName, vendorIdentifier, points, showBeforeEarned, repeatable, archived, gameCenterDetail, gameCenterGroup, groupAchievement, localizations, releases`

`fields[gameCenterDetails]`

`[string]`

Possible Values: `arcadeEnabled, challengeEnabled, app, gameCenterAppVersions, gameCenterGroup, gameCenterLeaderboards, gameCenterLeaderboardSets, gameCenterAchievements, defaultLeaderboard, defaultGroupLeaderboard, achievementReleases, leaderboardReleases, leaderboardSetReleases`

`fields[gameCenterGroups]`

`[string]`

Possible Values: `referenceName, gameCenterDetails, gameCenterLeaderboards, gameCenterLeaderboardSets, gameCenterAchievements`

`fields[gameCenterLeaderboardSets]`

`[string]`

Possible Values: `referenceName, vendorIdentifier, gameCenterDetail, gameCenterGroup, groupLeaderboardSet, localizations, gameCenterLeaderboards, releases`

`fields[gameCenterLeaderboards]`

`[string]`

Possible Values: `defaultFormatter, referenceName, vendorIdentifier, submissionType, scoreSortType, scoreRangeStart, scoreRangeEnd, recurrenceStartDate, recurrenceDuration, recurrenceRule, archived, gameCenterDetail, gameCenterGroup, groupLeaderboard, gameCenterLeaderboardSets, localizations, releases`

`include`

`[string]`

Possible Values: `gameCenterDetails, gameCenterLeaderboards, gameCenterLeaderboardSets, gameCenterAchievements`

`limit[gameCenterAchievements]`

`integer`

Maximum: `50`

`limit[gameCenterDetails]`

`integer`

Maximum: `50`

`limit[gameCenterLeaderboardSets]`

`integer`

Maximum: `50`

`limit[gameCenterLeaderboards]`

`integer`

Maximum: `50`

## Response Codes

` 200 ``OK`

GameCenterGroupResponse

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

### Reading Game Center details

Read the state of Game Center for an app

Get Game Center detail information for an app.

Read Game Center details

Read a specific Game Center detail and related information.

Read app versions for a Game Center detail

Get a list of app versions for a Game Center detail.

