

- Model I/O
-  MDLAnimatedVector3 

Class

# MDLAnimatedVector3

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class MDLAnimatedVector3
```

## Topics

### Instance Properties

var double3Array: [SIMD3&lt;Double>]

var float3Array: [SIMD3&lt;Float>]

### Instance Methods

func double3Value(atTime: TimeInterval) -> vector_double3

func float3Value(atTime: TimeInterval) -> vector_float3

func reset(double3Array: [SIMD3&lt;Double>], atTimes: [TimeInterval])

func reset(float3Array: [SIMD3&lt;Float>], atTimes: [TimeInterval])

func setDouble3(vector_double3, atTime: TimeInterval)

func setFloat3(vector_float3, atTime: TimeInterval)

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

