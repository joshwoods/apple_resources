

- App Store Connect API
-  Read the image for a specific achievement localization 

Web Service Endpoint

# Read the image for a specific achievement localization

Read the achievement image associated with specific localized information.

App Store Connect API 3.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/gameCenterAchievementLocalizations/{id}/gameCenterAchievementImage
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Apps resource. Obtain the app resource ID from the List all localizations for an achievement response.

## Query Parameters

`fields[gameCenterAchievementImages]`

`[string]`

Possible Values: `fileSize, fileName, imageAsset, uploadOperations, assetDeliveryState, gameCenterAchievementLocalization`

`fields[gameCenterAchievementLocalizations]`

`[string]`

Possible Values: `locale, name, beforeEarnedDescription, afterEarnedDescription, gameCenterAchievement, gameCenterAchievementImage`

`include`

`[string]`

Value: `gameCenterAchievementLocalization`

## Response Codes

` 200 ``OK`

GameCenterAchievementImageResponse

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
https://api.appstoreconnect.apple.com/v1/gameCenterAchievementLocalizations/ca329301-e7ad-4784-97cd-02faade43c2f/gameCenterAchievementImage
```

```
{
  “data” : {
    “type” : “gameCenterAchievementImages”,
    “id” : “38e6d9a7-9cbf-45f8-8246-1ef4728aecda”,
    “attributes” : {
      “fileSize” : 357407,
      “fileName” : “coffee1.png”,
      “imageAsset” : {
        “templateUrl” : “https://isq11.mzstatic.com/image/thumb/PurpleSource113/v4/64/14/07/641407e3-602f-ce23-10b8-c91b1762986c/38e6d9a7-9cbf-45f8-8246-1ef4728aecda_coffee1.png/{w}x{h}bb.{f}”,
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
      “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievementImages/38e6d9a7-9cbf-45f8-8246-1ef4728aecda”
    }
  },
  “links” : {
    “self” : “https://api.appstoreconnect.apple.com/v1/gameCenterAchievementLocalizations/ca329301-e7ad-4784-97cd-02faade43c2f/gameCenterAchievementImage”
  }

```

## See Also

### Reading achievements localizations

List all localizations for an achievement

Read information about the release for specific achievement.

Read achievement localization information

Read localized information for a specific locale for a specific achievement.

Read the achievement localization information

Read the achievement associated with specific localized information.

