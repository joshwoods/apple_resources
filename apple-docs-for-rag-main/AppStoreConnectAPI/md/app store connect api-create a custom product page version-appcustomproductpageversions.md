

- App Store Connect API
-  Create a custom product page version 

Web Service Endpoint

# Create a custom product page version

Add a version for your app custom product page.

App Store Connect API 1.7+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/appCustomProductPageVersions
```

## HTTP Body

AppCustomProductPageVersionCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

AppCustomProductPageVersionResponse

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

Read custom product page version information

Get information about a specific app custom product page version.

List custom product page versions

List the versions for a custom product page version.

List custom product pages localizations

List all localizations for an app custom product page.

Modify a custom product page version

Update the name and visibility status of an app custom product page.

