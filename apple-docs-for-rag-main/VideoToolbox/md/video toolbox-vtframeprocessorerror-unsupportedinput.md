

- Video Toolbox
- VTFrameProcessorError
-  unsupportedInput 

Type Property

# unsupportedInput

One or more frames is in a format which isn’t supported by the processor.

Mac Catalyst 13.0+macOS 10.8+

``` source
static var unsupportedInput: VTFrameProcessorError.Code { get }
```

## See Also

### Errors

static var fatalError: VTFrameProcessorError.Code

A fatal error occurred during processing.

static var initializationFailed: VTFrameProcessorError.Code

The session failed to initialize the processing pipeline.

static var invalidFrameTiming: VTFrameProcessorError.Code

A provided frame object has a presentation time stamp which isn’t supported by the processor.

static var invalidParameterError: VTFrameProcessorError.Code

A provided parameter isn’t valid.

static var memoryAllocationFailure: VTFrameProcessorError.Code

The session or processor is unable to allocate the required memory.

static var processingError: VTFrameProcessorError.Code

The processor encountered an issue that prevents it from processing the provided frame.

static var revisionNotSupported: VTFrameProcessorError.Code

The specified revision isn’t supported by the configured processor.

static var sessionAlreadyActive: VTFrameProcessorError.Code

An attempt is made to start a session that is already started.

static var sessionLevelError: VTFrameProcessorError.Code

The processing failed and current session should be stopped.

static var sessionNotStarted: VTFrameProcessorError.Code

The session is used to process frames without being started.

static var unknownError: VTFrameProcessorError.Code

The processor failed for an unknown reason.

static var unsupportedResolution: VTFrameProcessorError.Code

The processor failed due to an unsupported resolution.

