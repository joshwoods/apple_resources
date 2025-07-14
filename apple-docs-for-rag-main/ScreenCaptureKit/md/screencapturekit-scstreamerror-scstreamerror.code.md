

- ScreenCaptureKit
- SCStreamError
-  SCStreamError.Code 

Enumeration

# SCStreamError.Code

Codes for user cancellation events and errors that can occur in ScreenCaptureKit.

Mac Catalyst 18.2+macOS 12.3+

``` source
enum Code
```

## Topics

### User cancellation

case userStopped

An error message that indicates the user stopped the stream.

### Privacy and entitlements

case userDeclined

An error message that indicates the user didn’t grant Screen Recording permission to your app.

case missingEntitlements

An error message that indicates missing entitlements in your app.

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

case failedToStartMicrophoneCapture

An error message that indicates microphone capture failed to start.

case systemStoppedStream

An error message that indicates the system stopped the stream.

case internalError

An error message that indicates a stream can’t start due to a failure in ScreenCaptureKit’s internals.

### Shareable content

case noCaptureSource

An error message that indicates a stream doesn’t have a source to capture.

case noDisplayList

An error message that indicates a stream doesn’t have displays available.

case noWindowList

An error message that indicates a stream doesn’t have windows available.

case failedApplicationConnectionInvalid

An error message that indicates the stream lost its connection to an app.

case failedApplicationConnectionInterrupted

An error message that indicates there was an interruption in a connection to an app.

case failedNoMatchingApplicationContext

An error message that indicates there isn’t a matching app context for streaming.

### Invalid parameters

case invalidParameter

An error message that indicates an operation failed because of an invalid parameter value.

### Creating an error

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

