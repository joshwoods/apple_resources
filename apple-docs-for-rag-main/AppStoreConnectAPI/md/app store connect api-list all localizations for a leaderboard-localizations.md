

- App Store Connect API
-  List all localizations for a leaderboard 

Web Service Endpoint

# List all localizations for a leaderboard

Get a list of localized metadata for a leaderboard.

App Store Connect API 3.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboards/{id}/localizations
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the leaderboard resource ID from the Read leaderboard information response.

## Query Parameters

`fields[gameCenterLeaderboardImages]`

`[string]`

Possible Values: `fileSize, fileName, imageAsset, uploadOperations, assetDeliveryState, gameCenterLeaderboardLocalization`

`fields[gameCenterLeaderboardLocalizations]`

`[string]`

Possible Values: `locale, name, formatterOverride, formatterSuffix, formatterSuffixSingular, gameCenterLeaderboard, gameCenterLeaderboardImage`

`fields[gameCenterLeaderboards]`

`[string]`

Possible Values: `defaultFormatter, referenceName, vendorIdentifier, submissionType, scoreSortType, scoreRangeStart, scoreRangeEnd, recurrenceStartDate, recurrenceDuration, recurrenceRule, archived, gameCenterDetail, gameCenterGroup, groupLeaderboard, gameCenterLeaderboardSets, localizations, releases`

`include`

`[string]`

Possible Values: `gameCenterLeaderboard, gameCenterLeaderboardImage`

`limit`

`integer`

Maximum: `200`

## Response Codes

` 200 ``OK`

GameCenterLeaderboardLocalizationsResponse

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
https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboards/9b999364-308b-4ca3-8214-0af6cf5a6d51/localizations
```

```
{
  “data” : [ {
    “type” : “gameCenterLeaderboardLocalizations”,
    “id” : “9b999364-308b-4ca3-8214-0af6cf5a6d51”,
    “attributes” : {
      “locale” : “en-CA”,
      “name” : “Best Latte Art”,
      “formatterOverride” : “INTEGER”,
      “formatterSuffix” : “points”,
      “formatterSuffixSingular” : “points”
    },
    “relationships” : {
      “gameCenterLeaderboardImage” : {
        “links” : {
          “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboardLocalizations/9b999364-308b-4ca3-8214-0af6cf5a6d51/relationships/gameCenterLeaderboardImage”,
          “related” : “https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboardLocalizations/9b999364-308b-4ca3-8214-0af6cf5a6d51/gameCenterLeaderboardImage”
        }
      }
    },
    “links” : {
      “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboardLocalizations/9b999364-308b-4ca3-8214-0af6cf5a6d51”
    }
  }, {
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
  } ],
  “links” : {
    “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboards/843189c3-61a6-480a-a9d2-760a41299829/localizations”
  },
  “meta” : {
    “paging” : {
      “total” : 2,
      “limit” : 50
    }
  }
}

```

## See Also

### Managing leaderboard localizations

Read leaderboard localization information

Get information about a leaderboard localization.

Read the image for a leaderboard localization

Get information about the image associated with a leaderboard localization.

Create a leaderboard localization

Add a new leaderboard localization.

Modify a leaderboard localization

Edit a leaderboard localization.

Delete a leaderboard localization

Delete a localization that’s associated with a leaderboard.

