

- App Store Connect API
-  Modify an App Preview 

Web Service Endpoint

# Modify an App Preview

Commit the app preview after uploading it, and update the poster frame timecode.

App Store Connect API 1.2+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/appPreviews/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## HTTP Body

AppPreviewUpdateRequest

Content-Type: application/json

## Response Codes

` 200 ``OK`

AppPreviewResponse

`OK`

Content-Type: application/json

` 400 ``Bad Request`

ErrorResponse

`Bad Request`

An error occurred with your request.

Content-Type: application/json

` 401 ``Unauthorized`

ErrorResponse

`Unauthorized`

Content-Type: application/json

` 403 ``Forbidden`

ErrorResponse

`Forbidden`

Request not authorized.

Content-Type: application/json

` 404 ``Not Found`

ErrorResponse

`Not Found`

Resource not found.

Content-Type: application/json

` 409 ``Conflict`

ErrorResponse

`Conflict`

The provided resource data is not valid.

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## See Also

### Creating, Modifying, and Deleting App Previews

Create an App Preview

Add a new app preview to a preview set.

Delete an App Preview

Delete an app preview within a preview set.

