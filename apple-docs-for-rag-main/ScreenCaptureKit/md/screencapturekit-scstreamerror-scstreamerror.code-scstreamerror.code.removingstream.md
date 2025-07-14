

- ScreenCaptureKit
- SCStreamError
- SCStreamError.Code
-  SCStreamError.Code.removingStream 

Case

# SCStreamError.Code.removingStream

An error message that indicates a stream wasn’t removed.

Mac Catalyst 15.4+macOS 12.3+

``` source
case removingStream
```

## See Also

### Stream management

case attemptToStartStreamState

An error message that indicates a stream is already running or doesn’t exist when trying to start a stream.

case attemptToStopStreamState

An error message that indicates a stream is already stopped or doesn’t exist when trying to stop a stream.

case attemptToUpdateFilterState

An error message that indicates a stream couldn’t update its content filter.

case attemptToConfigState

An error message that indicates a stream couldn’t update its configuration.

case failedToStart

An error message that indicates a stream failed to start.

case failedToStartAudioCapture

An error message that indicates an audio stream failed to start.

case failedToStopAudioCapture

An error message that indicates an audio stream failed to stop.

case failedToStartMicrophoneCapture

An error message that indicates microphone capture failed to start.

case systemStoppedStream

An error message that indicates the system stopped the stream.

case internalError

An error message that indicates a stream can’t start due to a failure in ScreenCaptureKit’s internals.

