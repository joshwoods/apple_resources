

- App Store Connect API
-  Create an App Store Version Phased Release 

Web Service Endpoint

# Create an App Store Version Phased Release

Enable phased release for an App Store version.

App Store Connect API 1.2+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/appStoreVersionPhasedReleases
```

## HTTP Body

AppStoreVersionPhasedReleaseCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

AppStoreVersionPhasedReleaseResponse

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

## See Also

### Managing Phased Releases

Modify an App Store Version Phased Release

Pause or resume a phased release, or immediately release an app.

