

- App Store Connect API
-  Read leaderboard releases 

Web Service Endpoint

# Read leaderboard releases

List all leaderboard releases for a Game Center detail.

App Store Connect API 3.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/gameCenterDetails/{id}/leaderboardReleases
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[gameCenterDetails]`

`[string]`

Possible Values: `arcadeEnabled, challengeEnabled, app, gameCenterAppVersions, gameCenterGroup, gameCenterLeaderboards, gameCenterLeaderboardSets, gameCenterAchievements, defaultLeaderboard, defaultGroupLeaderboard, achievementReleases, leaderboardReleases, leaderboardSetReleases`

`fields[gameCenterLeaderboardReleases]`

`[string]`

Possible Values: `live, gameCenterDetail, gameCenterLeaderboard`

`fields[gameCenterLeaderboards]`

`[string]`

Possible Values: `defaultFormatter, referenceName, vendorIdentifier, submissionType, scoreSortType, scoreRangeStart, scoreRangeEnd, recurrenceStartDate, recurrenceDuration, recurrenceRule, archived, gameCenterDetail, gameCenterGroup, groupLeaderboard, gameCenterLeaderboardSets, localizations, releases`

`filter[gameCenterLeaderboard]`

`[string]`

`filter[live]`

`[string]`

`include`

`[string]`

Possible Values: `gameCenterDetail, gameCenterLeaderboard`

`limit`

`integer`

Maximum: `200`

## Response Codes

` 200 ``OK`

GameCenterLeaderboardReleasesResponse

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

### Reading and editing Game Center detail leaderboards

Read leaderboard information

Get all leaderboards and related information for a Game Center detail.

List leaderboards

​List all leaderboards for a Game Center detail.

