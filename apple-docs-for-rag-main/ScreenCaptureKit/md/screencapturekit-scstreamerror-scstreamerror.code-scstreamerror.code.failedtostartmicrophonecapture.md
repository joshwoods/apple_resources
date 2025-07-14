

- ScreenCaptureKit
- SCStreamError
- SCStreamError.Code
-  SCStreamError.Code.failedToStartMicrophoneCapture 

Case

# SCStreamError.Code.failedToStartMicrophoneCapture

An error message that indicates microphone capture failed to start.

Mac Catalyst 18.0+macOS 15.0+

``` source
case failedToStartMicrophoneCapture
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

case removingStream

An error message that indicates a stream wasn’t removed.

case failedToStartAudioCapture

An error message that indicates an audio stream failed to start.

case failedToStopAudioCapture

An error message that indicates an audio stream failed to stop.

case systemStoppedStream

An error message that indicates the system stopped the stream.

case internalError

An error message that indicates a stream can’t start due to a failure in ScreenCaptureKit’s internals.

