

- App Store Connect API
-  Create a leaderboard 

Web Service Endpoint

# Create a leaderboard

Add a new leaderboard to your app.

App Store Connect API 3.0+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboards
```

## HTTP Body

GameCenterLeaderboardCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

GameCenterLeaderboardResponse

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

App Store Connect API 3.7 release notes

## Discussion

### Example Request and Response

- Request
- Response

```
POST  https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboards-d 
{
    “data”: {
        “type”: “gameCenterLeaderboards”,
        “attributes”: {
            “referenceName”: “Cortado Temp LB”,
            “vendorIdentifier”: “CORTADOTEMP_LB”,
            “defaultFormatter”: “INTEGER”,
            “submissionType”: “BEST_SCORE”,
            “scoreSortType”: “DESC”,
            “scoreRangeStart”: “0”,
            “scoreRangeEnd”: “100”
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
    “type” : “gameCenterLeaderboards”,
    “id” : “8e76c29a-4d4d-4b1f-9389-0dd161cab83c”,
    “attributes” : {
      “defaultFormatter” : “INTEGER”,
      “referenceName” : “Cortado Temp LB”,
      “vendorIdentifier” : “CORTADOTEMP_LB”,
      “submissionType” : “BEST_SCORE”,
      “scoreSortType” : “DESC”,
      “scoreRangeStart” : “0”,
      “scoreRangeEnd” : “100”,
      “recurrenceStartDate” : null,
      “recurrenceDuration” : null,
      “recurrenceRule” : null,
      “archived” : false,
      “leaderboardType” : “CLASSIC”
    },
    “relationships” : {
      “groupLeaderboard” : {
        “links” : {
          “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboards/8e76c29a-4d4d-4b1f-9389-0dd161cab83c/relationships/groupLeaderboard”,
          “related” : “https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboards/8e76c29a-4d4d-4b1f-9389-0dd161cab83c/groupLeaderboard”
        }
      },
      “localizations” : {
        “links” : {
          “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboards/8e76c29a-4d4d-4b1f-9389-0dd161cab83c/relationships/localizations”,
          “related” : “https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboards/8e76c29a-4d4d-4b1f-9389-0dd161cab83c/localizations”
        }
      },
      “releases” : {
        “links” : {
          “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboards/8e76c29a-4d4d-4b1f-9389-0dd161cab83c/relationships/releases”,
          “related” : “https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboards/8e76c29a-4d4d-4b1f-9389-0dd161cab83c/releases”
        }
      },
      “leaderboardScores” : {
        “links” : {
          “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboards/8e76c29a-4d4d-4b1f-9389-0dd161cab83c/relationships/leaderboardScores”,
          “related” : “https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboards/8e76c29a-4d4d-4b1f-9389-0dd161cab83c/leaderboardScores”
        }
      }
    },
    “links” : {
      “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboards/8e76c29a-4d4d-4b1f-9389-0dd161cab83c”
    }
  },
  “links” : {
    “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboards”
  }
}
```

## See Also

### Creating, modifying, and deleting leaderboards

Edit a leaderboard

Modify the details of a leaderboard.

Edit the relationship between a leaderboard and a group leaderboard

Modify the group leadboard to which a leaderboard belongs.

Delete a leaderboard

Delete a leaderboard from your app.

