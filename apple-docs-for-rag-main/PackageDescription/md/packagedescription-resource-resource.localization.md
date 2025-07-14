

- PackageDescription
- Resource
-  Resource.Localization 

Enumeration

# Resource.Localization

Defines the explicit type of localization for resources.

SwiftPM 5.3+

``` source
enum Localization
```

## Topics

### Enumeration Cases

case base

A constant that represents base internationalization.

case `default`

A constant that represents default localization.

### Hashing

func hash(into: inout Hasher)

Hashes the localization by feeding the item into the given hasher.

var hashValue: Int

The localization’s hash value.

### Operator Functions

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Creating a Value

init?(rawValue: String)

Creates a new instance with the specified raw value.

### Accessing the Raw Value

var rawValue: String

The corresponding value of the raw type.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Applying Rules

static func process(String, localization: Resource.Localization?) -> Resource

Applies a platform-specific rules to the resource at the given path.

static func copy(String) -> Resource

Applies the copy rule to a resource at the given path.

