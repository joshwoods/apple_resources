

- App Store Connect API
-  List achievement releases 

Web Service Endpoint

# List achievement releases 

Read information about the achievement releases for specific Game Center detail.

App Store Connect API 3.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/gameCenterDetails/{id}/achievementReleases
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

`fields[gameCenterDetails]`

`[string]`

Possible Values: `arcadeEnabled, challengeEnabled, app, gameCenterAppVersions, gameCenterGroup, gameCenterLeaderboards, gameCenterLeaderboardSets, gameCenterAchievements, defaultLeaderboard, defaultGroupLeaderboard, achievementReleases, leaderboardReleases, leaderboardSetReleases`

`filter[gameCenterAchievement]`

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
https://api.appstoreconnect.apple.com/v1/gameCenterDetails/83b895ff-7bfe-5056-1208-ffd0d6a74e46/achievementReleases?limit=5
```

```
{
  “data” : [ {
    “type” : “gameCenterAchievementReleases”,
    “id” : “24d3a649-59e7-7d15-f794-3abf4e44d0a8”,
    “attributes” : {
      “live” : true
    },
    “links” : {
      “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievementReleases/24d3a649-59e7-7d15-f794-3abf4e44d0a8”
    }
  }, {
    “type” : “gameCenterAchievementReleases”,
    “id” : “71002ec8-e7e0-fc5f-456b-c2b563b3294d”,
    “attributes” : {
      “live” : true
    },
    “links” : {
      “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievementReleases/71002ec8-e7e0-fc5f-456b-c2b563b3294d”
    }
  }, {
    “type” : “gameCenterAchievementReleases”,
    “id” : “2025e5d2-d60f-7504-099a-c6d7df11292d”,
    “attributes” : {
      “live” : true
    },
    “links” : {
      “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievementReleases/2025e5d2-d60f-7504-099a-c6d7df11292d”
    }
  }, {
    “type” : “gameCenterAchievementReleases”,
    “id” : “b9d99cb3-c5f4-3050-f4dc-d6f4b749cba3”,
    “attributes” : {
      “live” : true
    },
    “links” : {
      “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievementReleases/b9d99cb3-c5f4-3050-f4dc-d6f4b749cba3”
    }
  }, {
    “type” : “gameCenterAchievementReleases”,
    “id” : “701b76ef-9fe5-f1e7-02ea-b875fe27d0fd”,
    “attributes” : {
      “live” : true
    },
    “links” : {
      “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievementReleases/701b76ef-9fe5-f1e7-02ea-b875fe27d0fd”
    }
  },
  “links” : {
    “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterDetails/83b895ff-7bfe-5056-1208-ffd0d6a74e46/achievementReleases?limit=5”
  },
  “meta” : {
    “paging” : {
      “total” : 35,
      “limit” : 5
    }
  }
}

```

## See Also

### Managing Game Center achievement releases

Read release information for an achievement

Read the state of an achievement release and related information.

Read Game Center achievement release information

Read the state of a specific achievement release.

Create a Game Center achievement release

Create a release for an achievement and a Game Center detail.

Delete a Game Center achievement release

Delete a release of an achievement or Game Center detail.

