

- App Store Connect API
-  List leaderboard sets in a group leaderboard set 

Web Service Endpoint

# List leaderboard sets in a group leaderboard set

List information about leaderboards and leaderboard sets in a group leaderboard set.

App Store Connect API 3.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboardSets/{id}/groupLeaderboardSet
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

`include`

`[string]`

Possible Values: `gameCenterDetail, gameCenterGroup, groupLeaderboardSet, localizations, gameCenterLeaderboards, releases`

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

GameCenterLeaderboardSetResponse

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

### Reading leaderboard sets

Read leaderboard set information

Read information about a specific leaderboard set.

List leaderboard information for a leaderboard set

Read the leadboards that belong to a learderboard set.

List all localizations for a leaderboard set

Get a list of localized metadata for a leaderboard set.

Read the leaderboards in a leaderboard set

List all leaderboards in a leaderboard set.

Read the group leaderboard set in a leaderboard set

List all the group leaderboard sets in a leaderboard set.

List releases for a leaderboard set

Read the state of releases for a leaderboard set and related information.

