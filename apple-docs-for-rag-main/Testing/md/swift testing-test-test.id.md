

- Swift Testing
- Test
-  Test.ID 

Structure

# Test.ID

A type representing the stable identity of the entity associated with an instance.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
struct ID
```

## Topics

### Operators

static func == (Test.ID, Test.ID) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

var moduleName: String

The name of the module containing the corresponding test.

var nameComponents: [String]

The fully qualified name components (other than the module name) used to identify the corresponding test.

var parent: Test.ID?

The ID of the parent test.

var sourceLocation: SourceLocation?

The source location of the corresponding test.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

CustomStringConvertible Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

