

- App Store Connect API
-  Read a specific App Encryption Declaration Document 

Web Service Endpoint

# Read a specific App Encryption Declaration Document

Get detailed information about a specified App Encryption Declaration document.

App Store Connect API 2.2+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appEncryptionDeclarationDocuments/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the app resource ID from the List App Encryption Declarations response, you will need to use the include `appEncryptionDeclarationDocument`

## Query Parameters

`fields[appEncryptionDeclarationDocuments]`

`[string]`

Possible Values: `fileSize, fileName, assetToken, downloadUrl, sourceFileChecksum, uploadOperations, assetDeliveryState`

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

## Discussion

### Example Request and Response

- Request
- Response

```
https://api.appstoreconnect.apple.com/v1/appEncryptionDeclarationDocuments/e55c4bbe-a1b9-427c-99cf-fd8db5050fc9
```

```
{  "data": {
    "type": "appEncryptionDeclarationDocuments",
    "id": "e55c4bbe-a1b9-427c-99cf-fd8db5050fc9",
    "attributes": {
      "fileSize": 186110,
      "fileName": "EncryptionDocumentation.pdf",
      "assetToken": "Purple113/v4/11/d4/08/11d408a8-e57a-4541-60bb-4192a3722623/e55c4bbe-a1b9-427c-99cf-fd8db5050fc9_EncryptionDocumentation.pdf",
      "downloadUrl": "https://misc-assets.itunes.apple.com/itunes-assets/Purple113/v4/11/d4/08/11d408a8-e57a-4541-60bb-4192a3722623/e55c4bbe-a1b9-427c-99cf-fd8db5050fc9_EncryptionDocumentation.pdf?accessKey=1675040844_8877869041959196296_dpXq9G7f4BF3oguy1BccshsmBYPlFP1xE4%2FenEAhRgymD2MPBYd1P%2BZopSavvkw3ZxuTRBGQwxHg4aBoWBl1UVFWOnW6nwI9Scivbm5vCk7GDEuVOImbEDaMYDC5Xxtag%2BVd2P4gDO7kdp%2FpPcnGLQFQ83RYrqfOqSqLstXnTwpbK9FPiQlGo1xIMZZYvLq5STbnREud24pbdmvvtUexlCoFuR7tjvpmRrlD0LGUUSs%3D",
      "sourceFileChecksum": "d228e04d46284ca195ad1ac7d13e269b",
      "uploadOperations": null,
      "assetDeliveryState": {
        "errors": [],
        "warnings": null,
        "state": "COMPLETE"
      }
    },
    "links": {
      "self": "https://api.appstoreconnect.apple.com/v1/appEncryptionDeclarationDocuments/e55c4bbe-a1b9-427c-99cf-fd8db5050fc9"
    }
  },
  "links": {
    "self": "https://api.appstoreconnect.apple.com/v1/appEncryptionDeclarationDocuments/e55c4bbe-a1b9-427c-99cf-fd8db5050fc9"
  }
}

```

## See Also

### Getting App Encryption Declarations

List App Encryption Declarations

Find and list all available app encryption declarations.

Read App Encryption Declaration Information

Get information about a specific app encryption declaration.

Read the App Information of an App Encryption Declaration

Get the app information from a specific app encryption declaration.

Deprecated

Read the Declaration Document for an App Encryption Declaration

Read the associate document for a specific App Encryption Declaration.

