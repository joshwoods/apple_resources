

- App Store Connect API
-  POST /v1/gameCenterLeaderboardEntrySubmissions 

Web Service Endpoint

# POST /v1/gameCenterLeaderboardEntrySubmissions

Add a new score for a player to a leaderboard.

App Store Connect API 3.2+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboardEntrySubmissions
```

## HTTP Body

GameCenterLeaderboardEntrySubmissionCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

GameCenterLeaderboardEntrySubmissionResponse

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
POST https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboardEntrySubmissions

{
  “data”: {
    “type”: “gameCenterLeaderboardEntrySubmissions”,
    “attributes”: {
      “score”: “123”,
      “scopedPlayerId”: “A:_5f21e308073d18f9b3afdc37f646e851”,
      “bundleId”: “com.apple.sample.actionship”,
      “vendorIdentifier”: “com.apple.sample.actionship.shipssank”
    }
  }
}
```

```
{
  “data”: {
    “type”: “gameCenterLeaderboardEntrySubmissions”,
    “id”: “3ef21559-006c-4308-831f-cd6cdd714863”,
    “attributes”: {
      “bundleId”: “com.apple.sample.actionship”,
      “challengeIds”: null,
      “context”: null,
      “scopedPlayerId”: “A:_5f21e308073d18f9b3afdc37f646e851”,
      “score”: “123”,
      “submittedDate”: null,
      “vendorIdentifier”: “com.apple.sample.actionship.shipssank”
    },
    “links”: {
      “self”: “https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboardEntrySubmissions/3ef21559-006c-4308-831f-cd6cdd714863”
    }
  },
  “links”: {
    “self”: “https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboardEntrySubmissions”
  }
}
```

