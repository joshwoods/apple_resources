

- Vision
-  VNTrackOpticalFlowRequest 

Class

# VNTrackOpticalFlowRequest

An object that determines the direction change of vectors for each pixel from a previous to current image.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
class VNTrackOpticalFlowRequest
```

## Overview

This request works at the pixel level, so both images must have the same dimensions to successfully perform the request.

Setting a region of interest isolates where to perform the change determination.

Important

Optical flow requests are very resource intensive, so perform only one request at a time. Release memory immediately after generating an optical flow.

## Topics

### Creating an Optical Flow

init()

Creates a new request that tracks the optical from one image to another.

init(completionHandler: VNRequestCompletionHandler?)

Creates a new request that tracks the optical from one image to another, with a system callback on completion.

### Configuring the Request

var computationAccuracy: VNTrackOpticalFlowRequest.ComputationAccuracy

The level of accuracy to compute the optical flow.

enum ComputationAccuracy

Computational accuracy options.

var keepNetworkOutput: Bool

A Boolean value that indicates the raw pixel buffer continues to emit from the network.

var outputPixelFormat: OSType

The pixel format type of the output value.

### Accessing the Results

var results: [VNPixelBufferObservation]?

The optical flow results the request observes.

## Relationships

### Inherits From

- VNStatefulRequest

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

class VNGenerateOpticalFlowRequest

An object that generates directional change vectors for each pixel in the targeted image.

