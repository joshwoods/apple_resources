

- Metal Performance Shaders Graph
-  MPSGraphPaddingMode 

Enumeration

# MPSGraphPaddingMode

The tensor padding mode.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
enum MPSGraphPaddingMode
```

## Topics

### Enumeration Cases

case antiPeriodic

Anti Periodic `x[-2] -> -x[L-3]`

case clampToEdge

ClampToEdge (PyTorch ReplicationPad)

case constant

Constant

case periodic

Periodic `x[-2] -> x[L-3], where L is size of x.`

case reflect

Reflect

case symmetric

Symmetric

case zero

Zero

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

