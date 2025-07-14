

- Shared With You Core
- SWPerson
-  SWPerson.Identity 

Class

# SWPerson.Identity

The unique identity for a person.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
class Identity
```

## Mentioned in 

Adding custom collaboration to your app

## Overview

This object represents an opaque Merkle tree where the root hash of the tree can uniquely identify the individual using the hash value of all of their devices. The individual’s devices use SWPerson.IdentityProof to prove themselves to be part of this identity, and can then be used for cryptographic signatures for that individual.

## Topics

### Creating a hash

init(rootHash: Data)

Creates and initializes the hash.

### Accessing the hash

var rootHash: Data

The root hash of the tree that represents the individual’s identity.

## Relationships

### Inherits From

- NSObject

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

class IdentityProof

An object that represents proof of inclusion to a Merkle tree.

class SignedIdentityProof

The signature that the system creates by signing the data with this person’s identity.

