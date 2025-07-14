

- App Store Connect API
-  POST /v1/gameCenterPlayerAchievementSubmissions 

Web Service Endpoint

# POST /v1/gameCenterPlayerAchievementSubmissions

Add a new entry for a player’s score for a Game Center achievement.

App Store Connect API 3.2+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/gameCenterPlayerAchievementSubmissions
```

## HTTP Body

GameCenterPlayerAchievementSubmissionCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

GameCenterPlayerAchievementSubmissionResponse

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

## Mentioned in 

App Store Connect API 3.2 release notes

## Discussion

### Example Request and Response

- Request
- Response

```
POST https://api.appstoreconnect.apple.com/v1/gameCenterPlayerAchievementSubmissions
{
  “data”: {
    “type”: “gameCenterPlayerAchievementSubmissions”,
    “attributes”: {
      “percentageAchieved”: 30,
      “scopedPlayerId”: “A:_5f21e308073d18f9b3afdc37f646e851”,
      “bundleId”: “com.apple.sample.actionship”,
      “vendorIdentifier”: “com.apple.sample.actionship.perfectaim”
    }
  }
}

```

```
{
  “data”: {
    “type”: “gameCenterPlayerAchievementSubmissions”,
    “id”: “d9f8b8dd-6050-45c6-a8e3-c6b97c186583”,
    “attributes”: {
      “bundleId”: “com.apple.sample.actionship”,
      “challengeIds”: null,
      “percentageAchieved”: 30,
      “scopedPlayerId”: “A:_5f21e308073d18f9b3afdc37f646e851”,
      “submittedDate”: null,
      “vendorIdentifier”: “com.apple.sample.actionship.perfectaim”
    },
    “links”: {
      “self”: “https://api.appstoreconnect.apple.com/v1/gameCenterPlayerAchievementSubmissions/d9f8b8dd-6050-45c6-a8e3-c6b97c186583”
    }
  },
  “links”: {
    “self”: “https://api.appstoreconnect.apple.com/v1/gameCenterPlayerAchievementSubmissions”
  }
}
```

