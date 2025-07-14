

- Metal
-  MTLReadWriteTextureTier 

Enumeration

# MTLReadWriteTextureTier

The support level for read-write texture formats.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
enum MTLReadWriteTextureTier
```

## Topics

### Enumeration Cases

case tier1

Tier 1 read/write textures are supported.

case tier2

Tier 2 read/write textures are supported.

case tierNone

Read-write textures are not supported.

### Initializers

init?(rawValue: UInt)

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

enum MTLShaderValidation

Indicates whether shader validation in an enabled or disabled state, or neither state.

enum MTLTransformType

