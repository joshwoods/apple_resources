

- App Store Connect API
-  Create an achievement image 

Web Service Endpoint

# Create an achievement image

Add a new achievement image.

App Store Connect API 3.0+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/gameCenterAchievementImages
```

## HTTP Body

GameCenterAchievementImageCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

GameCenterAchievementImageResponse

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

### Managing Game Center achievements images

Read achievement image information

Get information about an achievement image and its upload and processing status.

Modify an achievement image

Commit an achievement image after uploading it.

Delete an achievement image

Delete an image that’s associated with an achievement.

