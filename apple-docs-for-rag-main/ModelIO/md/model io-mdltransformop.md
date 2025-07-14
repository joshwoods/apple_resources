

- Model I/O
-  MDLTransformOp 

Protocol

# MDLTransformOp

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
protocol MDLTransformOp
```

## Topics

### Instance Properties

var name: String

**Required**

### Instance Methods

func double4x4(atTime: TimeInterval) -> matrix_double4x4

**Required**

func float4x4(atTime: TimeInterval) -> matrix_float4x4

**Required**

func isInverseOp() -> Bool

**Required**

## Relationships

### Conforming Types

- MDLTransformMatrixOp
- MDLTransformOrientOp
- MDLTransformRotateOp
- MDLTransformRotateXOp
- MDLTransformRotateYOp
- MDLTransformRotateZOp
- MDLTransformScaleOp
- MDLTransformTranslateOp

