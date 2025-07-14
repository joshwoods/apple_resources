

- App Store Connect API
-  Read the image for a leaderboard localization 

Web Service Endpoint

# Read the image for a leaderboard localization

Get information about the image associated with a leaderboard localization.

App Store Connect API 3.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboardLocalizations/{id}/gameCenterLeaderboardImage
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[gameCenterLeaderboardImages]`

`[string]`

Possible Values: `fileSize, fileName, imageAsset, uploadOperations, assetDeliveryState, gameCenterLeaderboardLocalization`

`fields[gameCenterLeaderboardLocalizations]`

`[string]`

Possible Values: `locale, name, formatterOverride, formatterSuffix, formatterSuffixSingular, gameCenterLeaderboard, gameCenterLeaderboardImage`

`include`

`[string]`

Value: `gameCenterLeaderboardLocalization`

## Response Codes

` 200 ``OK`

GameCenterLeaderboardImageResponse

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
https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboardLocalizations/5a75be8c-225a-4fd4-b51f-d33876c2c79b/gameCenterLeaderboardImage
```

```
{
  “data” : {
    “type” : “gameCenterLeaderboardImages”,
    “id” : “482f6124-4570-43a0-aa5e-ec289ba6faf8”,
    “attributes” : {
      “fileSize” : 357407,
      “fileName” : “coffee2.png”,
      “imageAsset” : {
        “templateUrl” : “https://isq11.mzstatic.com/image/thumb/PurpleSource113/v4/ad/e2/7b/ade27bd0-013d-86ef-2748-9d63b53e781e/482f6124-4570-43a0-aa5e-ec289ba6faf8_coffee2.png/{w}x{h}bb.{f}”,
        “width” : 512,
        “height” : 512
      },
      “uploadOperations” : [ ],
      “assetDeliveryState” : {
        “errors” : null,
        “warnings” : null,
        “state” : “COMPLETE”
      }
    },
    “links” : {
      “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboardImages/482f6124-4570-43a0-aa5e-ec289ba6faf8”
    }
  },
  “links” : {
    “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboardLocalizations/5a75be8c-225a-4fd4-b51f-d33876c2c79b/gameCenterLeaderboardImage”
  }
}
```

## See Also

### Managing leaderboard localizations

List all localizations for a leaderboard

Get a list of localized metadata for a leaderboard.

Read leaderboard localization information

Get information about a leaderboard localization.

Create a leaderboard localization

Add a new leaderboard localization.

Modify a leaderboard localization

Edit a leaderboard localization.

Delete a leaderboard localization

Delete a localization that’s associated with a leaderboard.

