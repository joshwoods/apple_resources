

- Model I/O
-  MDLAnimatedVector4 

Class

# MDLAnimatedVector4

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class MDLAnimatedVector4
```

## Topics

### Instance Properties

var double4Array: [SIMD4&lt;Double>]

var float4Array: [SIMD4&lt;Float>]

### Instance Methods

func double4Value(atTime: TimeInterval) -> vector_double4

func float4Value(atTime: TimeInterval) -> vector_float4

func reset(double4Array: [SIMD4&lt;Double>], atTimes: [TimeInterval])

func reset(float4Array: [SIMD4&lt;Float>], atTimes: [TimeInterval])

func setDouble4(vector_double4, atTime: TimeInterval)

func setFloat4(vector_float4, atTime: TimeInterval)

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

