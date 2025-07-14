

- Video Toolbox
- VTFrameProcessorError
- VTFrameProcessorError.Code
-  VTFrameProcessorError.Code.processingError 

Case

# VTFrameProcessorError.Code.processingError

The processor encountered an issue that prevents it from processing the provided frame.

Mac Catalyst 13.0+macOS 10.8+

``` source
case processingError
```

## See Also

### Enumeration Cases

case fatalError

A fatal error occurred during processing.

case initializationFailed

The session failed to initialize the processing pipeline.

case invalidFrameTiming

A provided frame object has a presentation time stamp which isn’t supported by the processor.

case invalidParameterError

A provided parameter isn’t valid.

case memoryAllocationFailure

The session or processor is unable to allocate the required memory.

case revisionNotSupported

The specified revision isn’t supported by the configured processor.

case sessionAlreadyActive

An attempt is made to start a session that is already started.

case sessionLevelError

The processing failed and current session should be stopped.

case sessionNotStarted

The session is used to process frames without being started.

case unknownError

The processor failed for an unknown reason.

case unsupportedInput

One or more frames is in a format which isn’t supported by the processor.

case unsupportedResolution

The processor failed due to an unsupported resolution.

