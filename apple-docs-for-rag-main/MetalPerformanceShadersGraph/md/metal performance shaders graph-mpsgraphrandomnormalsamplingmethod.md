

- Metal Performance Shaders Graph
-  MPSGraphRandomNormalSamplingMethod 

Enumeration

# MPSGraphRandomNormalSamplingMethod

The sampling method to use when generating values in the normal distribution.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
enum MPSGraphRandomNormalSamplingMethod
```

## Topics

### Enumeration Cases

case boxMuller

Use Box Muller transform to convert uniform values to values in the normal distribution. For bounded distributions this is a rejection sampling method.

case invCDF

Use inverse erf to convert uniform values to values in the normal distribution

### Initializers

init?(rawValue: UInt64)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

