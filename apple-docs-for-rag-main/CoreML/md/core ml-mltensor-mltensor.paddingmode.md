

- Core ML
- MLTensor
-  MLTensor.PaddingMode 

Enumeration

# MLTensor.PaddingMode

A mode that dictates how a tensor is padded.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
enum PaddingMode
```

## Topics

### Enumeration Cases

case constant(Float)

Pads the input tensor boundaries with a constant value.

case reflection

Pads the input tensor using the reflection of the input boundary.

case symmetric

Pads the input tensor using the reflection of the input, including the edge value.

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Equatable
- Hashable
- Sendable

