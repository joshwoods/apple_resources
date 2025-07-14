

- App Store Connect API
-  AppEncryptionDeclarationBuildsLinkagesRequest Deprecated

Object

# AppEncryptionDeclarationBuildsLinkagesRequest

A request body you use to add builds to an app encryption declaration.

App Store Connect API 1.0–2.4Deprecated

``` source
object AppEncryptionDeclarationBuildsLinkagesRequest
```

Deprecated

Use BuildUpdateRequest.Data.Relationships.AppEncryptionDeclaration instead.

## Properties

`data`

`[`AppEncryptionDeclarationBuildsLinkagesRequest.Data`]`

 (Required) 

The object types and IDs of the related resources.

## Topics

### Objects

object AppEncryptionDeclarationBuildsLinkagesRequest.Data

The data element of the request body.

## See Also

### Objects and Data Types

object AppEncryptionDeclarationCreateRequest

The request body you use to create an app encryption declaration.

object AppEncryptionDeclarationDocument

object AppEncryptionDeclarationDocumentCreateRequest

object AppEncryptionDeclarationDocumentResponse

object AppEncryptionDeclarationDocumentUpdateRequest

object AppEncryptionDeclaration

The data structure that represents an App Encryption Declarations resource.

object AppEncryptionDeclarationResponse

A response that contains a single App Encryption Declarations resource.

object AppEncryptionDeclarationWithoutIncludesResponse

object AppEncryptionDeclarationsResponse

A response that contains a list of App Encryption Declaration resources.

type AppEncryptionDeclarationState

Strings that represent the review or acceptance status of an app encryption declaration submitted to Apple.

