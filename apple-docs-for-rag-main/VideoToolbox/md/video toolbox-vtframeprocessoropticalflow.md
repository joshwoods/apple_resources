

- Video Toolbox
-  VTFrameProcessorOpticalFlow 

Class

# VTFrameProcessorOpticalFlow

A class to wrap bidirectional optical flow to send to the processor.

macOS 15.4+

``` source
class VTFrameProcessorOpticalFlow
```

## Overview

Instances retain the buffers backing them.

## Topics

### Creating an optical flow configuration

init?(forwardFlow: CVPixelBuffer, backwardFlow: CVPixelBuffer)

Creates an object with forward and backward optical flow pixel buffers.

### Inspecting the configuration

var backwardFlow: CVPixelBuffer

The backward optical flow pixel buffer that was provided when the object was created.

var forwardFlow: CVPixelBuffer

The forward optical flow pixel that was provided when the object was created.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Optical flow

class VTOpticalFlowConfiguration

A configuration object that enables optical flow on a frame processing session.

class VTOpticalFlowParameters

An object that describes frame-level optical flow parameters.

