

- App Store Connect API
-  List associated group achievement information for an achievement 

Web Service Endpoint

# List associated group achievement information for an achievement

Read information about the group for specific achievement.

App Store Connect API 3.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/{id}/groupAchievement
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the achievement resource ID from the List all achievements response.

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

`include`

`[string]`

Possible Values: `gameCenterDetail, gameCenterGroup, groupAchievement, localizations, releases`

`limit[localizations]`

`integer`

Maximum: `50`

`limit[releases]`

`integer`

Maximum: `50`

## Response Codes

` 200 ``OK`

GameCenterAchievementResponse

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

### Reading achievements

List all achievements

List all achievement information for a Game Center detail.

Read achievement information

Read information about a specific Game Center achievement.

List all localizations for an achievement

Read information about the release for specific achievement.

Read release information for an achievement

Read the state of an achievement release and related information.

List group achievements for an achievement

List associated group achievements for a specific achievement.

List achievement releases 

Read information about the achievement releases for specific Game Center detail.

