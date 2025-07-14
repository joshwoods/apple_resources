

- Shared With You Core
- SWPerson
-  SWPerson.SignedIdentityProof 

Class

# SWPerson.SignedIdentityProof

The signature that the system creates by signing the data with this person’s identity.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
class SignedIdentityProof
```

## Topics

### Creating a signed identity

init(personIdentityProof: SWPerson.IdentityProof, signatureData: Data)

Creates and intializes a signed identity object.

### Accessing signature data

var signatureData: Data

The signature the system creates by signing the data with this person’s identity.

## Relationships

### Inherits From

- SWPerson.IdentityProof

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

class IdentityProof

An object that represents proof of inclusion to a Merkle tree.

