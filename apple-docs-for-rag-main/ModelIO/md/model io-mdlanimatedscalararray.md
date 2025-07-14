

- Model I/O
-  MDLAnimatedScalarArray 

Class

# MDLAnimatedScalarArray

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class MDLAnimatedScalarArray
```

## Topics

### Initializers

init(elementCount: Int)

### Instance Properties

var doubleArray: [Double]

var elementCount: Int

var floatArray: [Float]

### Instance Methods

func doubleArray(atTime: TimeInterval) -> [Double]

func floatArray(atTime: TimeInterval) -> [Float]

func reset(doubleArray: [Double], atTimes: [TimeInterval])

func reset(floatArray: [Float], atTimes: [TimeInterval])

func set(doubleArray: [Double], atTime: TimeInterval)

func set(floatArray: [Float], atTime: TimeInterval)

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

