

- Metal
-  MTLShaderValidation 

Enumeration

# MTLShaderValidation

Indicates whether shader validation in an enabled or disabled state, or neither state.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
enum MTLShaderValidation
```

## Topics

### Validation States

case `default`

The default value when the property isn’t set.

case disabled

Disables shader validation.

case enabled

Enables shader validation.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Enumerations

enum MTLArgumentBuffersTier

The values that determine the limits and capabilities of argument buffers.

enum MTLLogStateError

enum MTLMathFloatingPointFunctions

Indicates which FP32 math functions Metal uses.

enum MTLMathMode

An indication of whether the compiler can perform optimizations for floating-point arithmetic that may violate the IEEE 754 standard.

enum MTLMatrixLayout

enum MTLReadWriteTextureTier

The support level for read-write texture formats.

enum MTLTransformType

