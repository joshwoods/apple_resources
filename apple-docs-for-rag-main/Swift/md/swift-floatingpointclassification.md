

- Swift
-  FloatingPointClassification 

Enumeration

# FloatingPointClassification

The IEEE 754 floating-point classes.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
enum FloatingPointClassification
```

## Topics

### Operators

static func == (FloatingPointClassification, FloatingPointClassification) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case negativeInfinity

A value equal to `-infinity`.

case negativeNormal

A negative value that uses the full precision of the floating-point type.

case negativeSubnormal

A negative, nonzero number that does not use the full precision of the floating-point type.

case negativeZero

A value equal to zero with a negative sign.

case positiveInfinity

A value equal to `+infinity`.

case positiveNormal

A positive value that uses the full precision of the floating-point type.

case positiveSubnormal

A positive, nonzero number that does not use the full precision of the floating-point type.

case positiveZero

A value equal to zero with a positive sign.

case quietNaN

A silent NaN (“not a number”) value.

case signalingNaN

A signaling NaN (“not a number”).

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Floating-Point Characteristics

enum FloatingPointRoundingRule

A rule for rounding a floating-point number.

enum FloatingPointSign

The sign of a floating-point value.

