

- Video Toolbox
-  VTFrameProcessorFrame 

Class

# VTFrameProcessorFrame

An object that wraps video frames to send to the processor, as source, reference, or output frames.

macOS 15.4+

``` source
class VTFrameProcessorFrame
```

## Overview

Instances retain the buffer backing them.

## Topics

### Create a frame object

init?(buffer: CVPixelBuffer, presentationTimeStamp: CMTime)

Creates a frame object with a pixel buffer and presentation time.

### Inspecting the frame

var buffer: CVPixelBuffer

The pixel buffer specified when the object was created.

var presentationTimeStamp: CMTime

The presentation timestamp specified when the object was created.

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

### Frame processor

class VTFrameProcessor

A class that creates a new frame processor for the configured video effect.

protocol VTFrameProcessorConfiguration

A protocol that describes the configuration of a processor to use during a video processing session.

protocol VTFrameProcessorParameters

The base protocol for input and output processing parameters for a frame processor implementation.

