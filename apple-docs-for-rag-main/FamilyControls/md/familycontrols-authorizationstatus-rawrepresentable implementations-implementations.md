

- FamilyControls
- AuthorizationStatus
-  RawRepresentable Implementations 

API Collection

# RawRepresentable Implementations

## Topics

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder, when the type’s `RawValue` is `Int`.

### Instance Properties

var hashValue: Int

The hashed value of the authorization status.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder, when the type’s `RawValue` is `Int`.

func hash(into: inout Hasher)

Hashes the essential components of the authorization status by feeding them into the given hash function.

