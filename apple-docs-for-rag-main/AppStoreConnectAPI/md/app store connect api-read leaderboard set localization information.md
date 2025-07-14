

- App Store Connect API
-  Read leaderboard set localization information 

Web Service Endpoint

# Read leaderboard set localization information

Get information about a leaderboard set localization.

App Store Connect API 3.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboardSetLocalizations/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[gameCenterLeaderboardSetImages]`

`[string]`

Possible Values: `fileSize, fileName, imageAsset, uploadOperations, assetDeliveryState, gameCenterLeaderboardSetLocalization`

`fields[gameCenterLeaderboardSetLocalizations]`

`[string]`

Possible Values: `locale, name, gameCenterLeaderboardSet, gameCenterLeaderboardSetImage`

`include`

`[string]`

Possible Values: `gameCenterLeaderboardSet, gameCenterLeaderboardSetImage`

## Response Codes

` 200 ``OK`

GameCenterLeaderboardSetLocalizationResponse

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

## See Also

### Managing leaderboard set localizations

Read the image associated with a leaderboard set localization

Get information about a leaderboard set image associated with a leaderboard set localization.

Create a leaderboard set localization

Add a new leaderboard set localization.

Modify a leaderboard set localization

Edit a leaderboard set localization.

Delete a leaderboard set localization

Delete a localization that’s associated with a leaderboard set.

