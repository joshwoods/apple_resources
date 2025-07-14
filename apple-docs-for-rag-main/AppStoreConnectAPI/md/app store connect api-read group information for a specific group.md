

- App Store Connect API
-  Read group information for a specific group 

Web Service Endpoint

# Read group information for a specific group

Read information for a specific group.

App Store Connect API 3.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/gameCenterGroups/{id}
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

### Managing groups

Read group information

List information for all groups.

Create a group

Add a new group.

Modify a group

Edit the reference name for a group.

Delete a group

Remove a group.

List the achievements in a group

List achievements information for a specific group.

List Game Center details for a group

Read Game Center detail information for a specific group.

List Game Center leaderboard sets in a group

Read Game Center leaderboard sets information for a specific group.

List Game Center leaderboards for a group

Read Game Center leaderboard information for a specific group.

