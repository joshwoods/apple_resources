

- FamilyControls
-  AuthorizationStatus 

Enumeration

# AuthorizationStatus

The status of your app’s authorization to provide parental controls.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
enum AuthorizationStatus
```

## Topics

### Determining the Status

case notDetermined

The app hasn’t requested authorization.

case denied

The user, parent, or guardian denied the request for authorization.

case approved

The user, parent, or guardian approved the request for authorization.

### Accessing the Raw Value

var rawValue: Int

The corresponding value of the raw type.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Debugging

var description: String

A nonlocalized description of the authorization value, suitable for debugging.

### Comparing Status Instances

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two authorization statuses aren’t equal.

var hashValue: Int

The hashed value of the authorization status.

func hash(into: inout Hasher)

Hashes the essential components of the authorization status by feeding them into the given hash function.

### Encoding Status Instances

func encode(to: any Encoder) throws

Encodes this value into the given encoder, when the type’s `RawValue` is `Int`.

### Creating Status

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder, when the type’s `RawValue` is `Int`.

init?(rawValue: Int)

Creates a new instance with the specified raw value.

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- RawRepresentable

## See Also

### Authorizations

class AuthorizationCenter

The center for requesting authorization to provide parental controls.

Family Controls

A Boolean value that indicates whether the app can request or revoke authorization to provide parental controls.

