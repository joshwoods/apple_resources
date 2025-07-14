

- Model I/O
-  MDLAnimatedScalar 

Class

# MDLAnimatedScalar

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class MDLAnimatedScalar
```

## Topics

### Instance Properties

var doubleArray: [Double]

var floatArray: [Float]

### Instance Methods

func doubleValue(atTime: TimeInterval) -> Double

func floatValue(atTime: TimeInterval) -> Float

func reset(doubleArray: [Double], atTimes: [TimeInterval])

func reset(floatArray: [Float], atTimes: [TimeInterval])

func setDouble(Double, atTime: TimeInterval)

func setFloat(Float, atTime: TimeInterval)

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

