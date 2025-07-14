

- Model I/O
-  MDLTransformStack 

Class

# MDLTransformStack

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class MDLTransformStack
```

## Topics

### Initializers

init()

### Instance Properties

var keyTimes: [NSNumber]

var transformOps: [any MDLTransformOp]

### Instance Methods

func addMatrixOp(String, inverse: Bool) -> MDLTransformMatrixOp

func addOrientOp(String, inverse: Bool) -> MDLTransformOrientOp

func addRotateOp(String, order: MDLTransformOpRotationOrder, inverse: Bool) -> MDLTransformRotateOp

func addRotateXOp(String, inverse: Bool) -> MDLTransformRotateXOp

func addRotateYOp(String, inverse: Bool) -> MDLTransformRotateYOp

func addRotateZOp(String, inverse: Bool) -> MDLTransformRotateZOp

func addScaleOp(String, inverse: Bool) -> MDLTransformScaleOp

func addTranslateOp(String, inverse: Bool) -> MDLTransformTranslateOp

func animatedValue(withName: String) -> MDLAnimatedValue

func count() -> Int

func double4x4(atTime: TimeInterval) -> matrix_double4x4

func float4x4(atTime: TimeInterval) -> matrix_float4x4

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- MDLComponent
- MDLTransformComponent
- NSCopying
- NSObjectProtocol

