

- App Store Connect API
-  Create a leaderboard localization 

Web Service Endpoint

# Create a leaderboard localization

Add a new leaderboard localization.

App Store Connect API 3.0+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboardLocalizations
```

## HTTP Body

GameCenterLeaderboardLocalizationCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

GameCenterLeaderboardLocalizationResponse

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

Use leaderboard formatters to specify the unit of measurement for a Game Center leaderboard. There is a new required attribute `defaultFormatter` when you use Create a leaderboard, which gives all your localizations the same formatter. You can also optionally use `formatterOverride` to override a specific leaderboard localization when calling Create a leaderboard localization or Modify a leaderboard localization.

Before App Store Connect API version 3.0, formatters were based on localizations and were required for each localization. Legacy leaderboards created before the new addition of the Game Center APIs will not have a `defaultFormatter` value, the value would be `null` in this case. Any localizations created before the new addition of the Game Center APIs will always have a `formatterOverride`.

### Example Request and Response

- Request
- Response

```
POST https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboardLocalizations -d 
{
    “data”: {
        “type”: “gameCenterLeaderboardLocalizations”,
        “attributes”: {
            “locale”: “en-US”,
            “name”: “Best Latte Art”,
            “formatterOverride”: “INTEGER”,
            “formatterSuffix”: “points”,
            “formatterSuffixSingular”: “point”
        },
        “relationships”: {
            “gameCenterLeaderboard”: {
                “data”: {
                    “type”: “gameCenterLeaderboards”,
                    “id”: “843189c3-61a6-480a-a9d2-760a41299829”
                }
            }
        }
    }
}
```

```
{
  “data” : {
    “type” : “gameCenterLeaderboardLocalizations”,
    “id” : “5a75be8c-225a-4fd4-b51f-d33876c2c79b”,
    “attributes” : {
      “locale” : “en-US”,
      “name” : “Best Latte Art”,
      “formatterOverride” : “INTEGER”,
      “formatterSuffix” : “points”,
      “formatterSuffixSingular” : “points”
    },
    “relationships” : {
      “gameCenterLeaderboardImage” : {
        “links” : {
          “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboardLocalizations/5a75be8c-225a-4fd4-b51f-d33876c2c79b/relationships/gameCenterLeaderboardImage”,
          “related” : “https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboardLocalizations/5a75be8c-225a-4fd4-b51f-d33876c2c79b/gameCenterLeaderboardImage”
        }
      }
    },
    “links” : {
      “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboardLocalizations/5a75be8c-225a-4fd4-b51f-d33876c2c79b”
    }
  },
  “links” : {
    “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboardLocalizations”
  }
}
```

## See Also

### Managing leaderboard localizations

List all localizations for a leaderboard

Get a list of localized metadata for a leaderboard.

Read leaderboard localization information

Get information about a leaderboard localization.

Read the image for a leaderboard localization

Get information about the image associated with a leaderboard localization.

Modify a leaderboard localization

Edit a leaderboard localization.

Delete a leaderboard localization

Delete a localization that’s associated with a leaderboard.

