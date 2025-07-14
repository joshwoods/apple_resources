

- App Store Connect API
-  Read Game Center details 

Web Service Endpoint

# Read Game Center details

Read a specific Game Center detail and related information.

App Store Connect API 3.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/gameCenterDetails/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the Game Center detail resource ID from the Read the state of Game Center for an app response.

## Query Parameters

`fields[gameCenterAchievementReleases]`

`[string]`

Possible Values: `live, gameCenterDetail, gameCenterAchievement`

`fields[gameCenterAchievements]`

`[string]`

Possible Values: `referenceName, vendorIdentifier, points, showBeforeEarned, repeatable, archived, gameCenterDetail, gameCenterGroup, groupAchievement, localizations, releases`

`fields[gameCenterAppVersions]`

`[string]`

Possible Values: `enabled, compatibilityVersions, appStoreVersion`

`fields[gameCenterDetails]`

`[string]`

Possible Values: `arcadeEnabled, challengeEnabled, app, gameCenterAppVersions, gameCenterGroup, gameCenterLeaderboards, gameCenterLeaderboardSets, gameCenterAchievements, defaultLeaderboard, defaultGroupLeaderboard, achievementReleases, leaderboardReleases, leaderboardSetReleases`

`fields[gameCenterGroups]`

`[string]`

Possible Values: `referenceName, gameCenterDetails, gameCenterLeaderboards, gameCenterLeaderboardSets, gameCenterAchievements`

`fields[gameCenterLeaderboardReleases]`

`[string]`

Possible Values: `live, gameCenterDetail, gameCenterLeaderboard`

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

Possible Values: `app, gameCenterAppVersions, gameCenterGroup, gameCenterLeaderboards, gameCenterLeaderboardSets, gameCenterAchievements, defaultLeaderboard, defaultGroupLeaderboard, achievementReleases, leaderboardReleases, leaderboardSetReleases`

`limit[achievementReleases]`

`integer`

Maximum: `50`

`limit[gameCenterAchievements]`

`integer`

Maximum: `50`

`limit[gameCenterAppVersions]`

`integer`

Maximum: `50`

`limit[gameCenterLeaderboardSets]`

`integer`

Maximum: `50`

`limit[gameCenterLeaderboards]`

`integer`

Maximum: `50`

`limit[leaderboardReleases]`

`integer`

Maximum: `50`

`limit[leaderboardSetReleases]`

`integer`

Maximum: `50`

## Response Codes

` 200 ``OK`

GameCenterDetailResponse

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

Read app versions for a Game Center detail

Get a list of app versions for a Game Center detail.

Read the groups in a Game Center detail

Get a list of groups in a Game Center detail.

