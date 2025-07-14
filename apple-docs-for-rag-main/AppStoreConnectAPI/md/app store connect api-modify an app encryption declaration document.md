

- App Store Connect API
-  Modify an App Encryption Declaration Document 

Web Service Endpoint

# Modify an App Encryption Declaration Document

Commit an App Encryption Declaration Document after uploading it.

App Store Connect API 2.2+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/appEncryptionDeclarationDocuments/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the app resource ID from the List App Encryption Declarations response, you will need to use the include `appEncryptionDeclarationDocument.`

## HTTP Body

AppEncryptionDeclarationDocumentUpdateRequest

Content-Type: application/json

## Response Codes

` 200 ``OK`

AppEncryptionDeclarationDocumentResponse

`OK`

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

` 404 ``Not Found`

ErrorResponse

`Not Found`

Content-Type: application/json

` 409 ``Conflict`

ErrorResponse

`Conflict`

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## See Also

### Uploading App Encryption Declaration Documents

Upload an App Encryption Declaration Document

Add an App Encryption Declaration Document to an existing App Encryption Declaration.

