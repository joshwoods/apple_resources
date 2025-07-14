

- App Store Connect API
-  Create a leaderboard image 

Web Service Endpoint

# Create a leaderboard image

Add a new leaderboard image.

App Store Connect API 3.0+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboardImages
```

## HTTP Body

GameCenterLeaderboardImageCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

GameCenterLeaderboardImageResponse

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

## See Also

### Managing leaderboard images

Read leaderboard image information

Get information about a leaderboard image and its upload and processing status.

Modify a leaderboard image

Commit a leaderboard image after uploading it.

Delete a leaderboard image

Delete an image that’s associated with a leaderboard.

