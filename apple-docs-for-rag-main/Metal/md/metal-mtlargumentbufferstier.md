

- Metal
-  MTLArgumentBuffersTier 

Enumeration

# MTLArgumentBuffersTier

The values that determine the limits and capabilities of argument buffers.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
enum MTLArgumentBuffersTier
```

## Overview

See Improving CPU Performance by Using Argument Buffers for more information about argument buffer tiers, limits, and capabilities. Query the argumentBuffersSupport property to determine argument buffer tier support for a given device.

## Topics

### Enumeration Cases

case tier1

Support for tier 1 argument buffers.

case tier2

Support for tier 2 argument buffers.

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

enum MTLLogStateError

enum MTLMathFloatingPointFunctions

Indicates which FP32 math functions Metal uses.

enum MTLMathMode

An indication of whether the compiler can perform optimizations for floating-point arithmetic that may violate the IEEE 754 standard.

enum MTLMatrixLayout

enum MTLReadWriteTextureTier

The support level for read-write texture formats.

enum MTLShaderValidation

Indicates whether shader validation in an enabled or disabled state, or neither state.

enum MTLTransformType

