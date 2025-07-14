

- Model I/O
-  MDLAnimatedQuaternion 

Class

# MDLAnimatedQuaternion

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
class MDLAnimatedQuaternion
```

## Topics

### Instance Properties

var doubleQuaternionArray: [simd_quatd]

var floatQuaternionArray: [simd_quatf]

### Instance Methods

func doubleQuaternionValue(atTime: TimeInterval) -> simd_quatd

func floatQuaternionValue(atTime: TimeInterval) -> simd_quatf

func reset(doubleQuaternionArray: [simd_quatd], atTimes: [TimeInterval])

func reset(floatQuaternionArray: [simd_quatf], atTimes: [TimeInterval])

func setDoubleQuaternion(simd_quatd, atTime: TimeInterval)

func setFloatQuaternion(simd_quatf, atTime: TimeInterval)

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

