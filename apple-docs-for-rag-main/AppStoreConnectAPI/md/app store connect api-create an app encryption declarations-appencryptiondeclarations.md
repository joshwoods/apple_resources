

- App Store Connect API
-  Create an app encryption declarations 

Web Service Endpoint

# Create an app encryption declarations

Add an app encryption delcaration for a specific app.

App Store Connect API 3.6+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/appEncryptionDeclarations
```

## HTTP Body

AppEncryptionDeclarationCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

AppEncryptionDeclarationResponse

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

## Mentioned in 

App Store Connect API 3.6 release notes

## See Also

### Assigning App Encryption Declarations

Assign Builds to an App Encryption Declaration

Assign one or more builds to an app encryption declaration.

Deprecated

