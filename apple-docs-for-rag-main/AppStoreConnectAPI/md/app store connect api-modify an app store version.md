

- App Store Connect API
-  Modify an App Store Version 

Web Service Endpoint

# Modify an App Store Version

Update the app store version for a specific app.

App Store Connect API 1.2+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/appStoreVersions/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## HTTP Body

AppStoreVersionUpdateRequest

Content-Type: application/json

## Response Codes

` 200 ``OK`

AppStoreVersionResponse

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

## Mentioned in 

Configuring alternative marketplaces and alternative marketplace apps

App Store Connect API 3.3 release notes

## See Also

### Creating and Modifying App Store Versions

Create an App Store Version

Add a new App Store version or platform to an app.

Delete an App Store Version

Delete an app store version that is associated with an app.

