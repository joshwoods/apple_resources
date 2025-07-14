

- Metal Performance Shaders Graph
-  MPSGraphRandomDistribution 

Enumeration

# MPSGraphRandomDistribution

The distributions supported by random operations.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
enum MPSGraphRandomDistribution
```

## Topics

### Enumeration Cases

case normal

The normal distribution defined by mean and standard deviation.

case truncatedNormal

The normal distribution defined by mean and standard deviation, truncated to the range \[min, max)

case uniform

The uniform distribution, with samples drawn uniformly from \[min, max) for float types, and \[min, max\] for integer types.

### Initializers

init?(rawValue: UInt64)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

