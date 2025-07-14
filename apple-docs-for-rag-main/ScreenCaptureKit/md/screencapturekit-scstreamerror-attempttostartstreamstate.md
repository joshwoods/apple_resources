

- ScreenCaptureKit
- SCStreamError
-  attemptToStartStreamState 

Type Property

# attemptToStartStreamState

An error message that indicates a stream is already running or doesn’t exist when trying to start a stream.

Mac Catalyst 15.4+macOS 12.3+

``` source
static var attemptToStartStreamState: SCStreamError.Code { get }
```

## See Also

### Stream management

static var attemptToStopStreamState: SCStreamError.Code

An error message that indicates a stream is already stopped or doesn’t exist when trying to stop a stream.

static var attemptToUpdateFilterState: SCStreamError.Code

An error message that indicates a stream couldn’t update its content filter.

static var attemptToConfigState: SCStreamError.Code

An error message that indicates a stream couldn’t update its configuration.

static var failedToStart: SCStreamError.Code

An error message that indicates a stream failed to start.

static var failedToStartAudioCapture: SCStreamError.Code

An error message that indicates an audio stream failed to start.

static var failedToStopAudioCapture: SCStreamError.Code

An error message that indicates an audio stream failed to stop.

static var failedToStartMicrophoneCapture: SCStreamError.Code

An error message that indicates microphone capture failed to start.

static var systemStoppedStream: SCStreamError.Code

An error message that indicates the system stopped the stream.

static var internalError: SCStreamError.Code

An error message that indicates a stream can’t start due to a failure in ScreenCaptureKit’s internals.

static var removingStream: SCStreamError.Code

An error message that indicates a stream wasn’t removed.

