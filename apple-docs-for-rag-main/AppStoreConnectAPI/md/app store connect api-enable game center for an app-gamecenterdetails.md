

- App Store Connect API
-  Enable Game Center for an app 

Web Service Endpoint

# Enable Game Center for an app

Create a Game Center detail for an app.

App Store Connect API 3.0+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/gameCenterDetails
```

## HTTP Body

GameCenterDetailCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

GameCenterDetailResponse

`Created`

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## Discussion

### Example Request and Response

- Request
- Response

```
https://api.appstoreconnect.apple.com/v1/gameCenterDetails -d
{
  “data”: {
    “type”: “gameCenterDetails”,
    “attributes”: {
      “challengeEnabled”: true
    },
    “relationships”: {
      “app”: {
        “data”: {
          “type”: “apps”,
          “id”: “6449448109”
        }
      }
    }
  }
}
```

```
{
  “data” : {
    “type” : “gameCenterDetails”,
    “id” : “6fd13854-b796-4cb5-87e1-9f2d15d3d7b9”,
    “attributes” : {
      “arcadeEnabled” : false,
      “challengeEnabled” : true
    },
    “relationships” : {
      “gameCenterAppVersions” : {
        “links” : {
          “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterDetails/6fd13854-b796-4cb5-87e1-9f2d15d3d7b9/relationships/gameCenterAppVersions”,
          “related” : “https://api.appstoreconnect.apple.com/v1/gameCenterDetails/6fd13854-b796-4cb5-87e1-9f2d15d3d7b9/gameCenterAppVersions”
        }
      },
      “gameCenterGroup” : {
        “links” : {
          “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterDetails/6fd13854-b796-4cb5-87e1-9f2d15d3d7b9/relationships/gameCenterGroup”,
          “related” : “https://api.appstoreconnect.apple.com/v1/gameCenterDetails/6fd13854-b796-4cb5-87e1-9f2d15d3d7b9/gameCenterGroup”
        }
      },
      “gameCenterLeaderboards” : {
        “links” : {
          “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterDetails/6fd13854-b796-4cb5-87e1-9f2d15d3d7b9/relationships/gameCenterLeaderboards”,
          “related” : “https://api.appstoreconnect.apple.com/v1/gameCenterDetails/6fd13854-b796-4cb5-87e1-9f2d15d3d7b9/gameCenterLeaderboards”
        }
      },
      “gameCenterLeaderboardSets” : {
        “links” : {
          “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterDetails/6fd13854-b796-4cb5-87e1-9f2d15d3d7b9/relationships/gameCenterLeaderboardSets”,
          “related” : “https://api.appstoreconnect.apple.com/v1/gameCenterDetails/6fd13854-b796-4cb5-87e1-9f2d15d3d7b9/gameCenterLeaderboardSets”
        }
      },
      “gameCenterAchievements” : {
        “links” : {
          “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterDetails/6fd13854-b796-4cb5-87e1-9f2d15d3d7b9/relationships/gameCenterAchievements”,
          “related” : “https://api.appstoreconnect.apple.com/v1/gameCenterDetails/6fd13854-b796-4cb5-87e1-9f2d15d3d7b9/gameCenterAchievements”
        }
      },
      “achievementReleases” : {
        “links” : {
          “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterDetails/6fd13854-b796-4cb5-87e1-9f2d15d3d7b9/relationships/achievementReleases”,
          “related” : “https://api.appstoreconnect.apple.com/v1/gameCenterDetails/6fd13854-b796-4cb5-87e1-9f2d15d3d7b9/achievementReleases”
        }
      },
      “leaderboardReleases” : {
        “links” : {
          “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterDetails/6fd13854-b796-4cb5-87e1-9f2d15d3d7b9/relationships/leaderboardReleases”,
          “related” : “https://api.appstoreconnect.apple.com/v1/gameCenterDetails/6fd13854-b796-4cb5-87e1-9f2d15d3d7b9/leaderboardReleases”
        }
      },
      “leaderboardSetReleases” : {
        “links” : {
          “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterDetails/6fd13854-b796-4cb5-87e1-9f2d15d3d7b9/relationships/leaderboardSetReleases”,
          “related” : “https://api.appstoreconnect.apple.com/v1/gameCenterDetails/6fd13854-b796-4cb5-87e1-9f2d15d3d7b9/leaderboardSetReleases”
        }
      },
      “blockedPlayers” : {
        “links” : {
          “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterDetails/6fd13854-b796-4cb5-87e1-9f2d15d3d7b9/relationships/blockedPlayers”,
          “related” : “https://api.appstoreconnect.apple.com/v1/gameCenterDetails/6fd13854-b796-4cb5-87e1-9f2d15d3d7b9/blockedPlayers”
        }
      }
    },
    “links” : {
      “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterDetails/6fd13854-b796-4cb5-87e1-9f2d15d3d7b9”
    }
  },
  “links” : {
    “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterDetails”
  }
}
```

## See Also

### Creating and editing Game Center details

Modify a Game Center detail for an app

Edit challenge state, default leaderboards, and groups.

Modify the associated leaderboard sets for a Game Center detail

Edit the associated leaderboard sets for a Game Center detail.

Modify the associated leaderboards for a Game Center detail

Edit the associated leaderboards for a Game Center detail.

