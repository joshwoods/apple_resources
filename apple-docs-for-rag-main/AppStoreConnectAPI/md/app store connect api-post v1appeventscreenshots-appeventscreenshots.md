

- App Store Connect API
-  POST /v1/appEventScreenshots 

Web Service Endpoint

# POST /v1/appEventScreenshots

App Store Connect API 1.7+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/appEventScreenshots
```

## HTTP Body

AppEventScreenshotCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

AppEventScreenshotResponse

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

### Endpoints

List the images for an in-app event

PATCH /v1/appEventScreenshots/{id}

Delete an App Event Screenshot

Delete a specific screenshot from an in-app event.

