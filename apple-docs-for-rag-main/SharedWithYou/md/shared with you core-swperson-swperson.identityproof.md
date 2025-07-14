

- Shared With You Core
- SWPerson
-  SWPerson.IdentityProof 

Class

# SWPerson.IdentityProof

An object that represents proof of inclusion to a Merkle tree.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
class IdentityProof
```

## Mentioned in 

Adding custom collaboration to your app

## Overview

This object represents an opaque Merkle tree proof of inclusion. Inclusion hashes are provided to verify that the individual device has access to the document.

## Topics

### Accessing attributes

var inclusionHashes: [Data]

The hashes of missing Merkle tree nodes that can provide proof of inclusion.

var publicKey: Data

The public key of local device.

var publicKeyIndex: Int

The index of the local public key in the Merkle tree.

## Relationships

### Inherits From

- NSObject

### Inherited By

- SWPerson.SignedIdentityProof

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Accessing attributes

class Identity

The unique identity for a person.

class SignedIdentityProof

The signature that the system creates by signing the data with this person’s identity.

