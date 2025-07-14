

- Model I/O
-  MDLAnimatedVector2 

Class

# MDLAnimatedVector2

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class MDLAnimatedVector2
```

## Topics

### Instance Properties

var double2Array: [SIMD2&lt;Double>]

var float2Array: [SIMD2&lt;Float>]

### Instance Methods

func double2Value(atTime: TimeInterval) -> vector_double2

func float2Value(atTime: TimeInterval) -> vector_float2

func reset(double2Array: [SIMD2&lt;Double>], atTimes: [TimeInterval])

func reset(float2Array: [SIMD2&lt;Float>], atTimes: [TimeInterval])

func setDouble2(vector_double2, atTime: TimeInterval)

func setFloat2(vector_float2, atTime: TimeInterval)

## Relationships

### Inherits From

- MDLAnimatedValue

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

