

- Assignables
- AnyUserIdentity
-  AnyUserIdentity.Error 

Enumeration

# AnyUserIdentity.Error

Error type for this user identity.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
enum Error
```

## Topics

### Decode error

case cannotDecode

Unable to decode the user identity.

### Operators

static func == (AnyUserIdentity.Error, AnyUserIdentity.Error) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

Error Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Inspecting an identity

var stringRepresentation: String

String representation of this user identity for display or debugging purposes.

var typeID: String

A unique type identifier for this user identity.

