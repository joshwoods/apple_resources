

- Vision
-  VNGenerateOpticalFlowRequest 

Class

# VNGenerateOpticalFlowRequest

An object that generates directional change vectors for each pixel in the targeted image.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class VNGenerateOpticalFlowRequest
```

## Overview

This request operates at a pixel level, so both images need to have the same dimensions to successfully perform the analysis. Setting a region of interest limits the region in which the analysis occurs. However, the system reports the resulting observation at full resolution.

Optical flow requests are resource-intensive, so create only one request at a time, and release it immediately after generating optical flows.

## Topics

### Configuring the Request

var computationAccuracy: VNGenerateOpticalFlowRequest.ComputationAccuracy

The accuracy level for computing optical flow.

enum ComputationAccuracy

The supported optical flow accuracy levels.

var outputPixelFormat: OSType

The output buffer’s pixel format.

var keepNetworkOutput: Bool

A Boolean value that indicates whether to keep the raw pixel buffer coming from the machine learning network.

### Accessing the Results

var results: [VNPixelBufferObservation]?

The results of the request to generate optical flow.

### Identifying Request Revisions

let VNGenerateOpticalFlowRequestRevision2: Int

A constant for specifying revision 2 of the optical flow generation request.

let VNGenerateOpticalFlowRequestRevision1: Int

A constant for specifying revision 1 of the optical flow generation request.

## Relationships

### Inherits From

- VNTargetedImageRequest

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Optical flow

class VNTrackOpticalFlowRequest

An object that determines the direction change of vectors for each pixel from a previous to current image.

