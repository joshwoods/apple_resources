

- App Store Connect API
-  List releases for a leaderboard 

Web Service Endpoint

# List releases for a leaderboard

Read the state of releases for a leaderboard and related information.

App Store Connect API 3.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboards/{id}/releases
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the leaderboard resource ID from the Read leaderboard information response.

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

`filter[gameCenterDetail]`

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

### Managing leaderboard releases

Read leaderboard release information

Read the state of a specific leaderboard release.

Create a leaderboard release

Add a new leaderboard release.

Delete a leaderboard release

Delete a new leaderboard release.

