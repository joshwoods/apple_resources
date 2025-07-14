

- PassKit (Apple Pay and Wallet)
-  PKAddPassMetadataPreview 

Class

# PKAddPassMetadataPreview

A preview object that contains information representing the pass you add to Wallet.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOSvisionOS 2.0+

``` source
class PKAddPassMetadataPreview
```

## Overview

Use this class to preview an object with all of the information you need to present a pass during provision.

## Topics

### Creating a preview of the pass

init(passThumbnail: CGImage, localizedDescription: String)

Provides a preview of an image object that represents the pass you add to Wallet.

var localizedDescription: String?

A localized description of the pass.

var passThumbnailImage: CGImage?

A CGImage object representing the card artwork of the pass you use during provisioning.

## Relationships

### Inherits From

- NSObject

### Inherited By

- PKShareablePassMetadata.Preview

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

class PKIdentityDocumentMetadata

A set of configured metadata defining the required information to add the corresponding pass to Wallet.

class PKIdentityNationalIDCardDescriptor

An object for requesting information from a user’s national ID card.

class PKJapanIndividualNumberCardMetadata

A class that contains metadata indicating the specific product instance to provision.

