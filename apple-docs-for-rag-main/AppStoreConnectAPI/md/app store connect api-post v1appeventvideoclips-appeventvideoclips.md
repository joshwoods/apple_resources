

- App Store Connect API
-  POST /v1/appEventVideoClips 

Web Service Endpoint

# POST /v1/appEventVideoClips

App Store Connect API 1.7+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/appEventVideoClips
```

## HTTP Body

AppEventVideoClipCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

AppEventVideoClipResponse

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

GET /v1/appEventVideoClips/{id}

PATCH /v1/appEventVideoClips/{id}

Delete an App Event Video Clip

Delete a specific video clip from an in-app event.

