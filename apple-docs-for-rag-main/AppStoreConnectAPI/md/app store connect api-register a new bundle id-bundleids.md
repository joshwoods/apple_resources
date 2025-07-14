

- App Store Connect API
-  Register a New Bundle ID 

Web Service Endpoint

# Register a New Bundle ID

Register a new bundle ID for app development.

App Store Connect API 1.1+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/bundleIds
```

## HTTP Body

BundleIdCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

BundleIdResponse

`Created`

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

The provided resource data is not valid.

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

