

- App Store Connect API
-  AppEncryptionDeclaration 

Object

# AppEncryptionDeclaration

The data structure that represents an App Encryption Declarations resource.

App Store Connect API 1.0+

``` source
object AppEncryptionDeclaration
```

## Properties

`attributes`

AppEncryptionDeclaration.Attributes

The resource’s attributes.

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the resource.

`relationships`

AppEncryptionDeclaration.Relationships

Navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `appEncryptionDeclarations`

`links`

ResourceLinks

Navigational links that include the self-link.

## Topics

### Objects

object AppEncryptionDeclaration.Attributes

Attributes that describe an App Encryption Declarations resource.

object AppEncryptionDeclaration.Relationships

The relationships you included in the request and those on which you can operate.

## See Also

### Objects and Data Types

object AppEncryptionDeclarationCreateRequest

The request body you use to create an app encryption declaration.

object AppEncryptionDeclarationDocument

object AppEncryptionDeclarationDocumentCreateRequest

object AppEncryptionDeclarationDocumentResponse

object AppEncryptionDeclarationDocumentUpdateRequest

object AppEncryptionDeclarationBuildsLinkagesRequest

A request body you use to add builds to an app encryption declaration.

Deprecated

object AppEncryptionDeclarationResponse

A response that contains a single App Encryption Declarations resource.

object AppEncryptionDeclarationWithoutIncludesResponse

object AppEncryptionDeclarationsResponse

A response that contains a list of App Encryption Declaration resources.

type AppEncryptionDeclarationState

Strings that represent the review or acceptance status of an app encryption declaration submitted to Apple.

