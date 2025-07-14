

- App Store Connect API
-  Create a leaderboard set image 

Web Service Endpoint

# Create a leaderboard set image

Add a new leaderboard set image.

App Store Connect API 3.0+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboardSetImages
```

## HTTP Body

GameCenterLeaderboardSetImageCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

GameCenterLeaderboardSetImageResponse

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

### Managing leaderboard set images

Read leaderboard set image information

Get information about a leaderboard set image and its upload and processing status.

Modify a leaderboard set image

Commit a leaderboard set image after uploading it.

Delete a leaderboard set image

Delete an image that’s associated with a leaderboard set.

