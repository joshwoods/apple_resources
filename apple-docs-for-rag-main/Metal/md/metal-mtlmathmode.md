

- Metal
-  MTLMathMode 

Enumeration

# MTLMathMode

An indication of whether the compiler can perform optimizations for floating-point arithmetic that may violate the IEEE 754 standard.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
enum MTLMathMode
```

## Topics

### Modes

case fast

An indicator of the mode the compiler uses to make aggressive, potentially lossy assumptions about floating-point math.

case relaxed

An indicator of the mode the compiler uses to make aggressive, potentially lossy assumptions about floating-point math, while honoring Inf/NaN.

case safe

An indicator of the mode the compiler uses to disable unsafe floating-point optimizations by preventing the compiler from making any transformations that could affect the results.

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

enum MTLMatrixLayout

enum MTLReadWriteTextureTier

The support level for read-write texture formats.

enum MTLShaderValidation

Indicates whether shader validation in an enabled or disabled state, or neither state.

enum MTLTransformType

