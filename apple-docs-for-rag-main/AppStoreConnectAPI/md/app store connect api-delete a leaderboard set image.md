

- App Store Connect API
-  Delete a leaderboard set image 

Web Service Endpoint

# Delete a leaderboard set image

Delete an image that’s associated with a leaderboard set.

App Store Connect API 3.0+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboardSetImages/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Response Codes

` 204 ``No Content`

`No Content`

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

## See Also

### Managing leaderboard set images

Read leaderboard set image information

Get information about a leaderboard set image and its upload and processing status.

Create a leaderboard set image

Add a new leaderboard set image.

Modify a leaderboard set image

Commit a leaderboard set image after uploading it.

