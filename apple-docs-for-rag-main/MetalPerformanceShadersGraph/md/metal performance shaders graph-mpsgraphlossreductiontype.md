

- Metal Performance Shaders Graph
-  MPSGraphLossReductionType 

Enumeration

# MPSGraphLossReductionType

The type of the reduction the graph applies in the loss operations.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
enum MPSGraphLossReductionType
```

## Topics

### Enumeration Cases

case mean

Reduces the loss down to a scalar with a mean operation.

case none

Computes the loss without reduction.

case sum

Reduces the loss down to a scalar with a sum operation.

### Initializers

init?(rawValue: UInt64)

### Type Properties

static var axis: MPSGraphLossReductionType

Computes the loss without reduction.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

