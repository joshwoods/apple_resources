

- App Store Connect API
-  Delete an achievement 

Web Service Endpoint

# Delete an achievement

Delete a specific achievement.

App Store Connect API 3.0+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the app resource ID from the List all achievements response.

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
DELETE https://api.appstoreconnect.apple.com/v1/gameCenterAchievements/082314fb-8b23-49db-b62a-08aad519e5aa
```

```
HTTP/1.1 204 No Content
```

## See Also

### Creating, modifying, and deleting achievements

Create an achievement

Add an achievement to a Game Center detail.

Modify an achievement

Modify properties for a specific achievement.

Modify the group for an achievement

Modify the achievement group for a specific achievement.

