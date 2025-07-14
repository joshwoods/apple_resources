

- App Store Connect API
-  Delete a Default App Clip Experience Image 

Web Service Endpoint

# Delete a Default App Clip Experience Image

Delete the image asset that appears on the App Clip card for a default App Clip experience.

App Store Connect API 1.6+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/appClipHeaderImages/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the App Clip Header Images resource.

## Response Codes

` 204 ``No Content`

`No Content`

The request completed successfully and the specific App Clip Header Images resource was deleted.

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

## See Also

### Managing App Clip Card Images

Read the App Clip Card Image

Get the image that appears on the App Clip card of a default App Clip experience.

Create an App Clip Card Image for a Default App Clip Experience

Reserve an image asset that appears on the App Clip card of a default App Clip experience.

Modify an App Clip Card Image

Change the image that appears on the App Clip card of a default App Clip experience.

