

- Vision
- VNGenerateOpticalFlowRequest
-  VNGenerateOpticalFlowRequest.ComputationAccuracy 

Enumeration

# VNGenerateOpticalFlowRequest.ComputationAccuracy

The supported optical flow accuracy levels.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
enum ComputationAccuracy
```

## Overview

The computation time typically increases with accuracy.

## Topics

### Accuracy Levels

case low

Low accuracy.

case medium

Medium accuracy.

case high

High accuracy.

case veryHigh

Very high accuracy.

### Creating an Accuracy Level

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

var computationAccuracy: VNGenerateOpticalFlowRequest.ComputationAccuracy

The accuracy level for computing optical flow.

var outputPixelFormat: OSType

The output buffer’s pixel format.

var keepNetworkOutput: Bool

A Boolean value that indicates whether to keep the raw pixel buffer coming from the machine learning network.

