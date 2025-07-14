

- Swift
-  FloatingPointRoundingRule 

Enumeration

# FloatingPointRoundingRule

A rule for rounding a floating-point number.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum FloatingPointRoundingRule
```

## Topics

### Operators

static func == (FloatingPointRoundingRule, FloatingPointRoundingRule) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case awayFromZero

Round to the closest allowed value whose magnitude is greater than or equal to that of the source.

case down

Round to the closest allowed value that is less than or equal to the source.

case toNearestOrAwayFromZero

Round to the closest allowed value; if two values are equally close, the one with greater magnitude is chosen.

case toNearestOrEven

Round to the closest allowed value; if two values are equally close, the even one is chosen.

case towardZero

Round to the closest allowed value whose magnitude is less than or equal to that of the source.

case up

Round to the closest allowed value that is greater than or equal to the source.

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

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Floating-Point Characteristics

enum FloatingPointClassification

The IEEE 754 floating-point classes.

enum FloatingPointSign

The sign of a floating-point value.

