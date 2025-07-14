

- App Store Connect API
-  Modify a leaderboard image 

Web Service Endpoint

# Modify a leaderboard image

Commit a leaderboard image after uploading it.

App Store Connect API 3.0+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboardImages/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## HTTP Body

GameCenterLeaderboardImageUpdateRequest

Content-Type: application/json

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## See Also

### Managing leaderboard images

Read leaderboard image information

Get information about a leaderboard image and its upload and processing status.

Create a leaderboard image

Add a new leaderboard image.

Delete a leaderboard image

Delete an image that’s associated with a leaderboard.

