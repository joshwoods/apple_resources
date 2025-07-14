

- PackageDescription
- Target
-  Target.TargetType 

Enumeration

# Target.TargetType

The different types of a target.

``` source
enum TargetType
```

## Topics

### Enumeration Cases

case regular

A target that contains code for the Swift package’s functionality.

case binary

A target that references a binary artifact.

case system

A target that adapts a library on the system to work with Swift packages.

case test

A target that contains tests for the Swift package’s other targets.

case executable

A target that contains code for an executable’s main module.

case plugin

A target that provides a package plug-in.

case macro

A target that provides a Swift macro.

### Creating a Value

init?(rawValue: String)

Creates a new instance with the specified raw value.

### Hashing

func hash(into: inout Hasher)

Hashes the target type by feeding the item into the given hasher.

var hashValue: Int

The target type’s hash value.

### Operator Functions

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

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

## See Also

### Describing the Target Type

var isTest: Bool

A Boolean value that indicates whether this is a test target.

let type: Target.TargetType

The type of the target.

