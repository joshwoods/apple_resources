

- PassKit (Apple Pay and Wallet)
-  PKIdentityDocumentMetadata 

Class

# PKIdentityDocumentMetadata

A set of configured metadata defining the required information to add the corresponding pass to Wallet.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOSvisionOS 2.0+

``` source
class PKIdentityDocumentMetadata
```

## Overview

Contains the required and optional metadata you need to configure a pass. Similar to PKShareablePassMetadata.

## Topics

### Instance Properties

var cardConfigurationIdentifier: String

var cardTemplateIdentifier: String

var credentialIdentifier: String

var serverEnvironmentIdentifier: String

var sharingInstanceIdentifier: String

## Relationships

### Inherits From

- NSObject

### Inherited By

- PKJapanIndividualNumberCardMetadata

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

class PKIdentityNationalIDCardDescriptor

An object for requesting information from a user’s national ID card.

class PKJapanIndividualNumberCardMetadata

A class that contains metadata indicating the specific product instance to provision.

