

- App Store Connect API
-  Read the Declaration Document for an App Encryption Declaration 

Web Service Endpoint

# Read the Declaration Document for an App Encryption Declaration

Read the associate document for a specific App Encryption Declaration.

App Store Connect API 2.2+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appEncryptionDeclarations/{id}/appEncryptionDeclarationDocument
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the app resource ID from the List App Encryption Declarations response.

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
https://api.appstoreconnect.apple.com/v1/appEncryptionDeclarations/6c2ddd3b-6d5e-4535-95f9-ece2c72c3848/appEncryptionDeclarationDocument
```

```
{
  "data" : {
    "type" : "appEncryptionDeclarationDocuments",
    "id" : "e55c4bbe-a1b9-427c-99cf-fd8db5050fc9",
    "attributes" : {
      "fileSize" : 186110,
      "fileName" : "EncryptionDocumentation.pdf",
      "assetToken" : "Purple113/v4/11/d4/08/11d408a8-e57a-4541-60bb-4192a3722623/e55c4bbe-a1b9-427c-99cf-fd8db5050fc9_EncryptionDocumentation.pdf",
      "downloadUrl" : "https://misc-assets.itunes.apple.com/itunes-assets/Purple113/v4/11/d4/08/11d408a8-e57a-4541-60bb-4192a3722623/e55c4bbe-a1b9-427c-99cf-fd8db5050fc9_EncryptionDocumentation.pdf?accessKey=1675044398_3481250329993679798_NHHQ2xtrY2EX3gS7CwgTVEwFSvYg1NO1KRtGg7LiuZQ9ASafREyyovMKVIm2AyCwWPHfd%2Fquw%2BrXJsN%2BAWBgKsOkNwTmjqrLA86eFDTPrajcum4yoziAitV%2BIiYH34nIreiGrF%2BMqePA%2FOijcxCGQH6Tle4YNoSb7q0B1SFcgFHUwCi9ML6hQIJ7AJyf2d4uJSouqy8zUWBwRDHBl2B0kpMj6BOSdY%2B22PiKpFQXweQ%3D",
      "sourceFileChecksum" : "d228e04d46284ca195ad1ac7d13e269b",
      "uploadOperations" : null,
      "assetDeliveryState" : {
        "errors" : [ ],
        "warnings" : null,
        "state" : "COMPLETE"
      }
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v1/appEncryptionDeclarationDocuments/e55c4bbe-a1b9-427c-99cf-fd8db5050fc9"
    }
  },
  "links" : {
    "self" : "https://api.appstoreconnect.apple.com/v1/appEncryptionDeclarations/6c2ddd3b-6d5e-4535-95f9-ece2c72c3848/appEncryptionDeclarationDocument"
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

Read a specific App Encryption Declaration Document

Get detailed information about a specified App Encryption Declaration document.

