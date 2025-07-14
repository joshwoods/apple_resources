

- Security
-  CMSSignedAttributes 

Structure

# CMSSignedAttributes

Optional attributes you can add to a signed message.

Mac Catalyst 13.0+macOS 10.0+

``` source
struct CMSSignedAttributes
```

## Overview

Use these flags with the CMSEncoderAddSignedAttributes(_:_:) method to cause the encoder to add attributes to a signed message that can be interpreted by the recipient. These attributes are not used for unsigned messages.

## Topics

### Attributes

static var attrSmimeCapabilities: CMSSignedAttributes

Identify signature, encryption, and digest algorithms supported by the encoder.

static var attrSmimeEncryptionKeyPrefs: CMSSignedAttributes

Indicate that the signing certificate included with the message is the preferred one for S/MIME encryption.

static var attrSmimeMSEncryptionKeyPrefs: CMSSignedAttributes

Indicate that the signing certificate included with the message is the preferred one for S/MIME encryption, but using an attribute object identifier (OID) preferred by Microsoft.

static var attrSigningTime: CMSSignedAttributes

Include the signing time.

static var attrAppleCodesigningHashAgility: CMSSignedAttributes

Include Apple codesigning hash agility.

static var attrAppleCodesigningHashAgilityV2: CMSSignedAttributes

Include Apple codesigning hash agility, version 2.

static var attrAppleExpirationTime: CMSSignedAttributes

Include the expiration time.

### Initializers

init(rawValue: UInt32)

Initializes a new attributes structure.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

