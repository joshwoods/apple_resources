

- App Store Connect API
-  Read leaderboard image information 

Web Service Endpoint

# Read leaderboard image information

Get information about a leaderboard image and its upload and processing status.

App Store Connect API 3.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboardImages/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[gameCenterLeaderboardImages]`

`[string]`

Possible Values: `fileSize, fileName, imageAsset, uploadOperations, assetDeliveryState, gameCenterLeaderboardLocalization`

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

## See Also

### Managing leaderboard images

Create a leaderboard image

Add a new leaderboard image.

Modify a leaderboard image

Commit a leaderboard image after uploading it.

Delete a leaderboard image

Delete an image that’s associated with a leaderboard.

