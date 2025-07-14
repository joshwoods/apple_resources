

- Metal Performance Shaders Graph
-  MPSGraphFFTScalingMode 

Enumeration

# MPSGraphFFTScalingMode

The scaling modes for Fourier transform operations.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
enum MPSGraphFFTScalingMode
```

## Topics

### Enumeration Cases

case none

Computes the FFT result with no scaling.

case size

Scales the FFT result with reciprocal of the total FFT size over all transformed dimensions.

case unitary

Scales the FFT result with reciprocal square root of the total FFT size over all transformed dimensions, resulting in signal strength conserving transformation.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

