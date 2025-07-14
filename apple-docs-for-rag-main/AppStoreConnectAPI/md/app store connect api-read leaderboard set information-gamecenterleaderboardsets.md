

- App Store Connect API
-  Read leaderboard set information 

Web Service Endpoint

# Read leaderboard set information

Get all leaderboard sets and related information for a Game Center detail.

App Store Connect API 3.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/gameCenterDetails/{id}/gameCenterLeaderboardSets
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[gameCenterDetails]`

`[string]`

Possible Values: `arcadeEnabled, challengeEnabled, app, gameCenterAppVersions, gameCenterGroup, gameCenterLeaderboards, gameCenterLeaderboardSets, gameCenterAchievements, defaultLeaderboard, defaultGroupLeaderboard, achievementReleases, leaderboardReleases, leaderboardSetReleases`

`fields[gameCenterGroups]`

`[string]`

Possible Values: `referenceName, gameCenterDetails, gameCenterLeaderboards, gameCenterLeaderboardSets, gameCenterAchievements`

`fields[gameCenterLeaderboardSetLocalizations]`

`[string]`

Possible Values: `locale, name, gameCenterLeaderboardSet, gameCenterLeaderboardSetImage`

`fields[gameCenterLeaderboardSetReleases]`

`[string]`

Possible Values: `live, gameCenterDetail, gameCenterLeaderboardSet`

`fields[gameCenterLeaderboardSets]`

`[string]`

Possible Values: `referenceName, vendorIdentifier, gameCenterDetail, gameCenterGroup, groupLeaderboardSet, localizations, gameCenterLeaderboards, releases`

`fields[gameCenterLeaderboards]`

`[string]`

Possible Values: `defaultFormatter, referenceName, vendorIdentifier, submissionType, scoreSortType, scoreRangeStart, scoreRangeEnd, recurrenceStartDate, recurrenceDuration, recurrenceRule, archived, gameCenterDetail, gameCenterGroup, groupLeaderboard, gameCenterLeaderboardSets, localizations, releases`

`filter[id]`

`[string]`

`filter[referenceName]`

`[string]`

`include`

`[string]`

Possible Values: `gameCenterDetail, gameCenterGroup, groupLeaderboardSet, localizations, gameCenterLeaderboards, releases`

`limit`

`integer`

Maximum: `200`

`limit[gameCenterLeaderboards]`

`integer`

Maximum: `50`

`limit[localizations]`

`integer`

Maximum: `50`

`limit[releases]`

`integer`

Maximum: `50`

## Response Codes

` 200 ``OK`

GameCenterLeaderboardSetsResponse

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

### Reading and editing leaderboard sets in a Game Center detail

List leaderboard sets

List all leaderboards for a Game Center detail.

Read leaderboard set release information

List all leaderboard set releases for a Game Center detail.

