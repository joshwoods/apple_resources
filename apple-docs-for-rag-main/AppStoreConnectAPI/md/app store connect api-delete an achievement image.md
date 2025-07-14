

- App Store Connect API
-  Delete an achievement image 

Web Service Endpoint

# Delete an achievement image

Delete an image that’s associated with an achievement.

App Store Connect API 3.0+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/gameCenterAchievementImages/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the game Center achievement images resource ID from the Read achievement information response.

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

## Discussion

### Example Request and Response

- Request
- Response

```
DELETE https://api.appstoreconnect.apple.com/v1/gameCenterAchievementImages/{id}
```

```
HTTP/1.1 204 No Content
```

## See Also

### Managing Game Center achievements images

Read achievement image information

Get information about an achievement image and its upload and processing status.

Create an achievement image

Add a new achievement image.

Modify an achievement image

Commit an achievement image after uploading it.

