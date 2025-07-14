

- App Store Connect API
-  Read leaderboard set image information 

Web Service Endpoint

# Read leaderboard set image information

Get information about a leaderboard set image and its upload and processing status.

App Store Connect API 3.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboardSetImages/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[gameCenterLeaderboardSetImages]`

`[string]`

Possible Values: `fileSize, fileName, imageAsset, uploadOperations, assetDeliveryState, gameCenterLeaderboardSetLocalization`

`include`

`[string]`

Value: `gameCenterLeaderboardSetLocalization`

## Response Codes

` 200 ``OK`

GameCenterLeaderboardSetImageResponse

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

### Managing leaderboard set images

Create a leaderboard set image

Add a new leaderboard set image.

Modify a leaderboard set image

Commit a leaderboard set image after uploading it.

Delete a leaderboard set image

Delete an image that’s associated with a leaderboard set.

