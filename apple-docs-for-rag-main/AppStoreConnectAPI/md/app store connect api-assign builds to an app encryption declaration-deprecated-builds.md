

- App Store Connect API
-  Assign Builds to an App Encryption Declaration Deprecated

Web Service Endpoint

# Assign Builds to an App Encryption Declaration

Assign one or more builds to an app encryption declaration.

App Store Connect API 1.0–2.4Deprecated

Deprecated

Use Modify a Build to update the relationship to an app encryption declaration instead.

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/appEncryptionDeclarations/{id}/relationships/builds
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the App Encryption Declarations resource ID from the List App Encryption Declarations response.

## HTTP Body

AppEncryptionDeclarationBuildsLinkagesRequest

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

### Assigning App Encryption Declarations

Create an app encryption declarations

Add an app encryption delcaration for a specific app.

