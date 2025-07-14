

- App Store Connect API
-  Read release information for an achievement 

Web Service Endpoint

# Read release information for an achievement

Read the state of an achievement release and related information.

App Store Connect API 3.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/{id}/releases
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the achievements resource ID from the List all achievements response.

## Query Parameters

`fields[gameCenterAchievementReleases]`

`[string]`

Possible Values: `live, gameCenterDetail, gameCenterAchievement`

`fields[gameCenterAchievements]`

`[string]`

Possible Values: `referenceName, vendorIdentifier, points, showBeforeEarned, repeatable, archived, gameCenterDetail, gameCenterGroup, groupAchievement, localizations, releases`

`fields[gameCenterDetails]`

`[string]`

Possible Values: `arcadeEnabled, challengeEnabled, app, gameCenterAppVersions, gameCenterGroup, gameCenterLeaderboards, gameCenterLeaderboardSets, gameCenterAchievements, defaultLeaderboard, defaultGroupLeaderboard, achievementReleases, leaderboardReleases, leaderboardSetReleases`

`filter[gameCenterDetail]`

`[string]`

`filter[live]`

`[string]`

`include`

`[string]`

Possible Values: `gameCenterDetail, gameCenterAchievement`

`limit`

`integer`

Maximum: `200`

## Response Codes

` 200 ``OK`

GameCenterAchievementReleasesResponse

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

## Discussion

### Example Request and Response

- Request
- Response

```
https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/4a6bcd3d-0325-418b-3bbf-671bd15be8c6/releases
```

```
{
  “data” : [ {
    “type” : “gameCenterAchievementReleases”,
    “id” : “be3bd01f-fd78-9093-63a7-bc25ff890eb2”,
    “attributes” : {
      “live” : true
    },
    “links” : {
      “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievementReleases/be3bd01f-fd78-9093-63a7-bc25ff890eb2”
    }
  } ],
  “links” : {
    “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/4a6bcd3d-0325-418b-3bbf-671bd15be8c6/releases”
  },
  “meta” : {
    “paging” : {
      “total” : 1,
      “limit” : 50
    }
  }
}
```

## See Also

### Managing Game Center achievement releases

List achievement releases 

Read information about the achievement releases for specific Game Center detail.

Read Game Center achievement release information

Read the state of a specific achievement release.

Create a Game Center achievement release

Create a release for an achievement and a Game Center detail.

Delete a Game Center achievement release

Delete a release of an achievement or Game Center detail.

