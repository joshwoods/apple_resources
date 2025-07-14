

- App Store Connect API
-  List the achievements in a group 

Web Service Endpoint

# List the achievements in a group

List achievements information for a specific group.

App Store Connect API 3.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/gameCenterGroups/{id}/gameCenterAchievements
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[gameCenterAchievementLocalizations]`

`[string]`

Possible Values: `locale, name, beforeEarnedDescription, afterEarnedDescription, gameCenterAchievement, gameCenterAchievementImage`

`fields[gameCenterAchievementReleases]`

`[string]`

Possible Values: `live, gameCenterDetail, gameCenterAchievement`

`fields[gameCenterAchievements]`

`[string]`

Possible Values: `referenceName, vendorIdentifier, points, showBeforeEarned, repeatable, archived, gameCenterDetail, gameCenterGroup, groupAchievement, localizations, releases`

`fields[gameCenterDetails]`

`[string]`

Possible Values: `arcadeEnabled, challengeEnabled, app, gameCenterAppVersions, gameCenterGroup, gameCenterLeaderboards, gameCenterLeaderboardSets, gameCenterAchievements, defaultLeaderboard, defaultGroupLeaderboard, achievementReleases, leaderboardReleases, leaderboardSetReleases`

`fields[gameCenterGroups]`

`[string]`

Possible Values: `referenceName, gameCenterDetails, gameCenterLeaderboards, gameCenterLeaderboardSets, gameCenterAchievements`

`filter[archived]`

`[string]`

`filter[id]`

`[string]`

`filter[referenceName]`

`[string]`

`include`

`[string]`

Possible Values: `gameCenterDetail, gameCenterGroup, groupAchievement, localizations, releases`

`limit`

`integer`

Maximum: `200`

`limit[localizations]`

`integer`

Maximum: `50`

`limit[releases]`

`integer`

Maximum: `50`

## Response Codes

` 200 ``OK`

GameCenterAchievementsResponse

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

Read group information for a specific group

Read information for a specific group.

Create a group

Add a new group.

Modify a group

Edit the reference name for a group.

Delete a group

Remove a group.

List Game Center details for a group

Read Game Center detail information for a specific group.

List Game Center leaderboard sets in a group

Read Game Center leaderboard sets information for a specific group.

List Game Center leaderboards for a group

Read Game Center leaderboard information for a specific group.

