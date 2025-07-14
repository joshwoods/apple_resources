

- App Store Connect API
-  Modify an achievement image 

Web Service Endpoint

# Modify an achievement image

Commit an achievement image after uploading it.

App Store Connect API 3.0+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/gameCenterAchievementImages/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the game Center achievement images resource ID from the Read achievement information response.

## HTTP Body

GameCenterAchievementImageUpdateRequest

Content-Type: application/json

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

Create an achievement image

Add a new achievement image.

Delete an achievement image

Delete an image that’s associated with an achievement.

