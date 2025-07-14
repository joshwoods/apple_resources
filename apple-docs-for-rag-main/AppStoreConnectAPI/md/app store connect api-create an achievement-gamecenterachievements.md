

- App Store Connect API
-  Create an achievement 

Web Service Endpoint

# Create an achievement

Add an achievement to a Game Center detail.

App Store Connect API 3.0+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/gameCenterAchievements
```

## HTTP Body

GameCenterAchievementCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

GameCenterAchievementResponse

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
POST https://api.appstoreconnect.apple.com/v1/gameCenterAchievements -d {
  “data”: {
    “type”: “gameCenterAchievements”,
    “attributes”: {
      “referenceName”: “Perfectly Steamed Milk Texture”,
      “vendorIdentifier”: “PSMT_ACH”,
      “points”: 0,
      “repeatable”: false,
      “showBeforeEarned”: false
    },
    “relationships”: {
      “gameCenterDetail”: {
        “data”: {
          “type”: “gameCenterDetails”,
          “id”: “6fd13854-b796-4cb5-87e1-9f2d15d3d7b9”
        }
      }
    }
  }
}
```

```
{
  “data” : {
    “type” : “gameCenterAchievements”,
    “id” : “304e0f56-63b2-492f-980e-bce6fafb8502”,
    “attributes” : {
      “referenceName” : “Perfectly Steamed Milk Texture”,
      “vendorIdentifier” : “PSMT_ACH”,
      “points” : 0,
      “showBeforeEarned” : false,
      “repeatable” : false,
      “archived” : false
    },
    “relationships” : {
      “groupAchievement” : {
        “links” : {
          “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/304e0f56-63b2-492f-980e-bce6fafb8502/relationships/groupAchievement”,
          “related” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/304e0f56-63b2-492f-980e-bce6fafb8502/groupAchievement”
        }
      },
      “localizations” : {
        “links” : {
          “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/304e0f56-63b2-492f-980e-bce6fafb8502/relationships/localizations”,
          “related” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/304e0f56-63b2-492f-980e-bce6fafb8502/localizations”
        }
      },
      “releases” : {
        “links” : {
          “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/304e0f56-63b2-492f-980e-bce6fafb8502/relationships/releases”,
          “related” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/304e0f56-63b2-492f-980e-bce6fafb8502/releases”
        }
      }
    },
    “links” : {
      “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/304e0f56-63b2-492f-980e-bce6fafb8502”
    }
  },
  “links” : {
    “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievements”
  }
}
```

## See Also

### Creating, modifying, and deleting achievements

Modify an achievement

Modify properties for a specific achievement.

Modify the group for an achievement

Modify the achievement group for a specific achievement.

Delete an achievement

Delete a specific achievement.

