

- Core Media
-  CMTimeRoundingMethod 

Enumeration

# CMTimeRoundingMethod

An enumeration of rounding methods to use when performing time calculations.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
enum CMTimeRoundingMethod
```

## Topics

### Default Rounding Method

static var `default`: CMTimeRoundingMethod

The default rounding method.

### Rounding Methods

case roundHalfAwayFromZero

Rounds half away from zero.

case roundAwayFromZero

Rounds away from zero.

case roundTowardZero

Rounds toward zero.

case quickTime

Rounds using the QuickTime method.

case roundTowardPositiveInfinity

Rounds toward positive infinity.

case roundTowardNegativeInfinity

Rounds toward negative infinity.

### Initializers

init?(rawValue: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Changing the Timescale

func CMTimeConvertScale(CMTime, timescale: Int32, method: CMTimeRoundingMethod) -> CMTime

Converts the source time to a new timescale using the specified rounding method.

