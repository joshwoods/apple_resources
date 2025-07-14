

- App Store Connect API
-  Upload an App Encryption Declaration Document 

Web Service Endpoint

# Upload an App Encryption Declaration Document

Add an App Encryption Declaration Document to an existing App Encryption Declaration.

App Store Connect API 2.2+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/appEncryptionDeclarationDocuments
```

## HTTP Body

AppEncryptionDeclarationDocumentCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

AppEncryptionDeclarationDocumentResponse

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

### Uploading App Encryption Declaration Documents

Modify an App Encryption Declaration Document

Commit an App Encryption Declaration Document after uploading it.

