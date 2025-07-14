

- Create ML
- MLDataValue
-  MLDataValue.ValueType 

Enumeration

# MLDataValue.ValueType

An enumeration describing the supported underlying types that an `MLDataValue wraps`.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
enum ValueType
```

## Topics

### Supported values

case int

An integer type.

case double

A double type.

case string

A string type.

case dictionary

A dictionary type.

case sequence

A sequence type.

case multiArray

A multidimensional type.

case invalid

An invalid type.

### Describing a data value type

var description: String

A text representation of the data value type.

var debugDescription: String

A text representation of the data value type that’s suitable for output during debugging.

### Comparing value types

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Operators

static func == (MLDataValue.ValueType, MLDataValue.ValueType) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

CustomDebugStringConvertible Implementations

CustomStringConvertible Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable

## See Also

### Inspecting the type

var type: MLDataValue.ValueType

The kind of the underlying value that the data value wraps.

