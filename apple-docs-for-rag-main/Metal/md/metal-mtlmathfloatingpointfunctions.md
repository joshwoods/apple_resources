

- Metal
-  MTLMathFloatingPointFunctions 

Enumeration

# MTLMathFloatingPointFunctions

Indicates which FP32 math functions Metal uses.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
enum MTLMathFloatingPointFunctions
```

## Topics

### Function Sets

case fast

An indication that Metal uses the fast version of the 32b floating-point math functions.

case precise

An indication that Metal uses the precise version of the 32b floating-point math functions.

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

enum MTLMathMode

An indication of whether the compiler can perform optimizations for floating-point arithmetic that may violate the IEEE 754 standard.

enum MTLMatrixLayout

enum MTLReadWriteTextureTier

The support level for read-write texture formats.

enum MTLShaderValidation

Indicates whether shader validation in an enabled or disabled state, or neither state.

enum MTLTransformType

