

- Video Toolbox
-  VTFrameProcessor 

Class

# VTFrameProcessor

A class that creates a new frame processor for the configured video effect.

macOS 15.4+

``` source
class VTFrameProcessor
```

## Overview

Use this class to perform frame by frame processing on your video. Start by specifying a video effect by passing a VTFrameProcessorConfiguration object to the startSession(configuration:) call. Once the session is created, process(parameters:completionHandler:) is called in a loop to process your video’s frames one at a time. Once all the frames are processed, call an endSession() to finish all pending processing.

For successful processing, the caller needs to ensure that all buffers passed to the processWithParameters interface are unmodified (including attachments) until the function returns or the callback is received in the case of asynchronous mode.

## Topics

### Creating a frame processor

init()

Creates a new frame processor.

### Processing frames

func startSession(configuration: any VTFrameProcessorConfiguration) throws

Starts a new session and configures the processor pipeline.

func process(parameters: any VTFrameProcessorParameters, completionHandler: (any VTFrameProcessorParameters, (any Error)?) -> Void)

Asynchronously performs the video effect specified in the start session.

func process(with: any MTLCommandBuffer, parameters: any VTFrameProcessorParameters)

Asynchronously performs the video effect specified in the start session specifically for Metal.

func endSession()

Performs all necessary tasks to end the session.

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

class VTFrameProcessorFrame

An object that wraps video frames to send to the processor, as source, reference, or output frames.

protocol VTFrameProcessorConfiguration

A protocol that describes the configuration of a processor to use during a video processing session.

protocol VTFrameProcessorParameters

The base protocol for input and output processing parameters for a frame processor implementation.

