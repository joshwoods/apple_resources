

- App Store Connect API
-  Create an achievement localization 

Web Service Endpoint

# Create an achievement localization

Add Game Center achievement localized information for a new locale.

App Store Connect API 3.0+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/gameCenterAchievementLocalizations
```

## HTTP Body

GameCenterAchievementLocalizationCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

GameCenterAchievementLocalizationResponse

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
POST https://api.appstoreconnect.apple.com/v1/gameCenterAchievementLocalizations -d {
    “data”: {
        “type”: “gameCenterAchievementLocalizations”,
        “attributes”: {
            “locale”: “en-US”,
            “name”: “Perfectly steamed milk”,
            “afterEarnedDescription”: “You did it! The milk had the perfect texture.”,
            “beforeEarnedDescription”: “You will earn this achievement upon steaming milk to the perfect texture.”
        },
        “relationships”: {
            “gameCenterAchievement”: {
                “data”: {
                    “type”: “gameCenterAchievements”,
                    “id”: “304e0f56-63b2-492f-980e-bce6fafb8502”
                }
            }
        }
    }
}
```

```
{
  “data” : {
    “type” : “gameCenterAchievementLocalizations”,
    “id” : “ca329301-e7ad-4784-97cd-02faade43c2f”,
    “attributes” : {
      “locale” : “en-US”,
      “name” : “Perfectly steamed milk”,
      “beforeEarnedDescription” : “You will earn this achievement upon steaming milk to the perfect texture.”,
      “afterEarnedDescription” : “You did it! The milk had the perfect texture.”
    },
    “relationships” : {
      “gameCenterAchievement” : {
        “links” : {
          “self” : “https://appstoreconnect.apple.com/v1/gameCenterAchievementLocalizations/ca329301-e7ad-4784-97cd-02faade43c2f/relationships/gameCenterAchievement”,
          “related” : “https://appstoreconnect.apple.com/v1/gameCenterAchievementLocalizations/ca329301-e7ad-4784-97cd-02faade43c2f/gameCenterAchievement”
        }
      },
      “gameCenterAchievementImage” : {
        “links” : {
          “self” : “https://appstoreconnect.apple.com/v1/gameCenterAchievementLocalizations/ca329301-e7ad-4784-97cd-02faade43c2f/relationships/gameCenterAchievementImage”,
          “related” : “https://appstoreconnect.apple.com/v1/gameCenterAchievementLocalizations/ca329301-e7ad-4784-97cd-02faade43c2f/gameCenterAchievementImage”
        }
      }
    },
    “links” : {
      “self” : “https://appstoreconnect.apple.com/v1/gameCenterAchievementLocalizations/ca329301-e7ad-4784-97cd-02faade43c2f”
    }
  },
  “links” : {
    “self” : “https://appstoreconnect.apple.com/v1/gameCenterAchievementLocalizations”
  }
}
```

## See Also

### Creating, modifying, and deleting achievements localizations

Edit an achievement localization

Modify localized Game Center achievement information for a particular language.

Delete an achievement localization

Delete localization metadata that’s associated with an achievement.

