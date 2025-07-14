

- Swift
-  FloatingPointSign 

Enumeration

# FloatingPointSign

The sign of a floating-point value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
enum FloatingPointSign
```

## Topics

### Operators

static func == (FloatingPointSign, FloatingPointSign) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case minus

The sign for a negative value.

case plus

The sign for a positive value.

### Initializers

init?(rawValue: Int)

Creates a new instance with the specified raw value.

### Instance Properties

var hashValue: Int

The hash value.

var rawValue: Int

The corresponding value of the raw type.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Aliases

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Floating-Point Characteristics

enum FloatingPointClassification

The IEEE 754 floating-point classes.

enum FloatingPointRoundingRule

A rule for rounding a floating-point number.

