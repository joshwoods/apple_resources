

- App Store Connect API
-  Assign the App Encryption Declaration for a Build Deprecated

Web Service Endpoint

# Assign the App Encryption Declaration for a Build

Assign an app encryption declaration to a build.

App Store Connect API 1.0+

Deprecated

Use Modify a Build to update the relationship to an app encryption declaration instead.

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/builds/{id}/relationships/appEncryptionDeclaration
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource.

## HTTP Body

BuildAppEncryptionDeclarationLinkageRequest

Content-Type: application/json

## Response Codes

` 204 ``No Content`

`No Content`

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

### Modifying Builds

Modify a Build

Expire a build or change its encryption exemption setting.

