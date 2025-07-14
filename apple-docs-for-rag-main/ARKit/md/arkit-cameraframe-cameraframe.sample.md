

- ARKit
- CameraFrame
-  CameraFrame.Sample 

Structure

# CameraFrame.Sample

Information that describes a sample from a camera frame.

visionOS 2.0+

``` source
struct Sample
```

## Overview

Use this structure to access information about a sample from a CameraFrame, such as the frame’s settings and parameters, a pixel buffer that contains the sample’s data, and so on.

## Topics

### Inspecting camera frame samples

var parameters: CameraFrame.Sample.Parameters

The frame’s parameters.

struct Parameters

A frame’s parameters, such as the camera type, intrinsics, timestamps, exposure, and so on.

var pixelBuffer: CVPixelBuffer

### Instance Properties

var description: String

A textual representation of this camera frame sample.

## Relationships

### Conforms To

- CustomStringConvertible
- Equatable
- Sendable

## See Also

### Getting camera frame information

var primarySample: CameraFrame.Sample

Gets the primary frame sample for a camera frame.

func sample(for: CameraFrameProvider.CameraPosition) -> CameraFrame.Sample?

Returns the camera frame sample for a given camera position.

var description: String

A textual representation of this camera frame.

