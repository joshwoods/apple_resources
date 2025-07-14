

- App Store Connect API
-  AppEncryptionDeclarationResponse 

Object

# AppEncryptionDeclarationResponse

A response that contains a single App Encryption Declarations resource.

App Store Connect API 1.0+

``` source
object AppEncryptionDeclarationResponse
```

## Properties

`data`

AppEncryptionDeclaration

 (Required) 

The resource data.

`links`

DocumentLinks

 (Required) 

Navigational links that include the self-link.

`included`

`[*]`

Possible types: App`, `Build`, `AppEncryptionDeclarationDocument

## See Also

### Related Documentation

Read App Encryption Declaration Information

Get information about a specific app encryption declaration.

### Objects and Data Types

object AppEncryptionDeclarationCreateRequest

The request body you use to create an app encryption declaration.

object AppEncryptionDeclarationDocument

object AppEncryptionDeclarationDocumentCreateRequest

object AppEncryptionDeclarationDocumentResponse

object AppEncryptionDeclarationDocumentUpdateRequest

object AppEncryptionDeclaration

The data structure that represents an App Encryption Declarations resource.

object AppEncryptionDeclarationBuildsLinkagesRequest

A request body you use to add builds to an app encryption declaration.

Deprecated

object AppEncryptionDeclarationWithoutIncludesResponse

object AppEncryptionDeclarationsResponse

A response that contains a list of App Encryption Declaration resources.

type AppEncryptionDeclarationState

Strings that represent the review or acceptance status of an app encryption declaration submitted to Apple.

