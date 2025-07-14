

- App Store Connect API
-  Read the achievement localization information 

Web Service Endpoint

# Read the achievement localization information

Read the achievement associated with specific localized information.

App Store Connect API 3.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/gameCenterAchievementLocalizations/{id}/gameCenterAchievement
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Apps resource. Obtain the app resource ID from the List all localizations for an achievement response.

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

### Reading achievements localizations

List all localizations for an achievement

Read information about the release for specific achievement.

Read achievement localization information

Read localized information for a specific locale for a specific achievement.

Read the image for a specific achievement localization

Read the achievement image associated with specific localized information.

