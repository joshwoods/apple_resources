

- Model I/O
-  MDLAnimatedVector3Array 

Class

# MDLAnimatedVector3Array

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class MDLAnimatedVector3Array
```

## Topics

### Initializers

init(elementCount: Int)

### Instance Properties

var double3Array: [SIMD3&lt;Double>]

var elementCount: Int

var float3Array: [SIMD3&lt;Float>]

### Instance Methods

func double3Array(atTime: TimeInterval) -> [SIMD3&lt;Double>]

func float3Array(atTime: TimeInterval) -> [SIMD3&lt;Float>]

func reset(double3Array: [SIMD3&lt;Double>], atTimes: [TimeInterval])

func reset(float3Array: [SIMD3&lt;Float>], atTimes: [TimeInterval])

func set(double3Array: [SIMD3&lt;Double>], atTime: TimeInterval)

func set(float3Array: [SIMD3&lt;Float>], atTime: TimeInterval)

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

