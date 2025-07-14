

- Model I/O
-  MDLAnimatedQuaternionArray 

Class

# MDLAnimatedQuaternionArray

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class MDLAnimatedQuaternionArray
```

## Topics

### Initializers

init(elementCount: Int)

### Instance Properties

var doubleQuaternionArray: [simd_quatd]

var elementCount: Int

var floatQuaternionArray: [simd_quatf]

### Instance Methods

func doubleQuaternionArray(atTime: TimeInterval) -> [simd_quatd]

func floatQuaternionArray(atTime: TimeInterval) -> [simd_quatf]

func reset(doubleQuaternionArray: [simd_quatd], atTimes: [TimeInterval])

func reset(floatQuaternionArray: [simd_quatf], atTimes: [TimeInterval])

func set(doubleQuaternionArray: [simd_quatd], atTime: TimeInterval)

func set(floatQuaternionArray: [simd_quatf], atTime: TimeInterval)

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

