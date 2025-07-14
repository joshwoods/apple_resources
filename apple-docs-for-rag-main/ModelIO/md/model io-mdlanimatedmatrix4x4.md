

- Model I/O
-  MDLAnimatedMatrix4x4 

Class

# MDLAnimatedMatrix4x4

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class MDLAnimatedMatrix4x4
```

## Topics

### Instance Properties

var double4x4Array: [double4x4]

var float4x4Array: [float4x4]

### Instance Methods

func double4x4Value(atTime: TimeInterval) -> matrix_double4x4

func float4x4Value(atTime: TimeInterval) -> matrix_float4x4

func reset(double4Array: [double4x4], atTimes: [TimeInterval])

func reset(float4x4Array: [float4x4], atTimes: [TimeInterval])

func setDouble4x4(matrix_double4x4, atTime: TimeInterval)

func setFloat4x4(matrix_float4x4, atTime: TimeInterval)

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

