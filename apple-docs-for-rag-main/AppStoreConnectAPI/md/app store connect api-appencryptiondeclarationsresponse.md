

- App Store Connect API
-  AppEncryptionDeclarationsResponse 

Object

# AppEncryptionDeclarationsResponse

A response that contains a list of App Encryption Declaration resources.

App Store Connect API 1.0+

``` source
object AppEncryptionDeclarationsResponse
```

## Properties

`data`

`[`AppEncryptionDeclaration`]`

 (Required) 

The resource data.

`links`

PagedDocumentLinks

 (Required) 

Navigational links that include the self-link.

`meta`

PagingInformation

Paging information.

`included`

`[*]`

Possible types: App`, `Build`, `AppEncryptionDeclarationDocument

## See Also

### Related Documentation

List App Encryption Declarations

Find and list all available app encryption declarations.

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

object AppEncryptionDeclarationResponse

A response that contains a single App Encryption Declarations resource.

object AppEncryptionDeclarationWithoutIncludesResponse

type AppEncryptionDeclarationState

Strings that represent the review or acceptance status of an app encryption declaration submitted to Apple.

