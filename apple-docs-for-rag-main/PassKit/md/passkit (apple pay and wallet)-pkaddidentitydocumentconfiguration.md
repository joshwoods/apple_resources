

- PassKit (Apple Pay and Wallet)
-  PKAddIdentityDocumentConfiguration 

Class

# PKAddIdentityDocumentConfiguration

Configuration to define the identity document.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOSvisionOS 2.0+

``` source
class PKAddIdentityDocumentConfiguration
```

## Overview

Use this class for identity document passes. You provide the underlying metadata that defines the passes.

## Topics

### Setting the metadata

var metadata: PKIdentityDocumentMetadata

A set of configurable metadata that defines the required information to add the corresponding pass to Wallet.

class func forMetadata(PKIdentityDocumentMetadata, completion: (PKAddIdentityDocumentConfiguration?, (any Error)?) -> Void)

Returns the identity document configuration.

## Relationships

### Inherits From

- PKAddSecureElementPassConfiguration

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

class PKAddPassMetadataPreview

A preview object that contains information representing the pass you add to Wallet.

class PKIdentityDocumentMetadata

A set of configured metadata defining the required information to add the corresponding pass to Wallet.

class PKIdentityNationalIDCardDescriptor

An object for requesting information from a user’s national ID card.

class PKJapanIndividualNumberCardMetadata

A class that contains metadata indicating the specific product instance to provision.

