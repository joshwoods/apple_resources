

- PassKit (Apple Pay and Wallet)
-  PKJapanIndividualNumberCardMetadata 

Class

# PKJapanIndividualNumberCardMetadata

A class that contains metadata indicating the specific product instance to provision.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOSvisionOS 2.0+

``` source
class PKJapanIndividualNumberCardMetadata
```

## Overview

This class is similar to PKShareablePassMetadata.

## Topics

### Initializing the digital card metadata

init(provisioningCredentialIdentifier: String, sharingInstanceIdentifier: String, cardConfigurationIdentifier: String, preview: PKAddPassMetadataPreview)

Initializes the user instance for provisioning.

init(provisioningCredentialIdentifier: String, sharingInstanceIdentifier: String, cardTemplateIdentifier: String, preview: PKAddPassMetadataPreview)

Initializes the product instance to provision.

### Defining configuration

var authenticationPassword: String?

A string that specifies the authentication password when provisioning the pass.

var preview: PKAddPassMetadataPreview

An object that contains information representing the pass for provisioning.

var signingPassword: String?

A string that sets the signing password when you provision the pass.

## Relationships

### Inherits From

- PKIdentityDocumentMetadata

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Japan passes

struct JPKIPassContents

A set of actions for viewing and updating PINs, passwords, and signing abilities associated with digital identities on the JPKI applet.

class PKAddIdentityDocumentConfiguration

Configuration to define the identity document.

class PKAddPassMetadataPreview

A preview object that contains information representing the pass you add to Wallet.

class PKIdentityDocumentMetadata

A set of configured metadata defining the required information to add the corresponding pass to Wallet.

class PKIdentityNationalIDCardDescriptor

An object for requesting information from a user’s national ID card.

