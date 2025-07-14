

- Vision
- VNTrackOpticalFlowRequest
-  VNTrackOpticalFlowRequest.ComputationAccuracy 

Enumeration

# VNTrackOpticalFlowRequest.ComputationAccuracy

Computational accuracy options.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
enum ComputationAccuracy
```

## Topics

### Options

case low

An option that indicates a low level of computational accuracy.

case medium

An option that indicates a moderate level of computational accuracy.

case high

An option that indicates a high level of computational accuracy.

case veryHigh

An option that indicates a very high level of computational accuracy.

case low

An option that indicates a low level of computational accuracy.

case medium

An option that indicates a moderate level of computational accuracy.

case high

An option that indicates a high level of computational accuracy.

case veryHigh

An option that indicates a very high level of computational accuracy.

### Creating an Accuracy Option

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring the Request

var computationAccuracy: VNTrackOpticalFlowRequest.ComputationAccuracy

The level of accuracy to compute the optical flow.

var keepNetworkOutput: Bool

A Boolean value that indicates the raw pixel buffer continues to emit from the network.

var outputPixelFormat: OSType

The pixel format type of the output value.

