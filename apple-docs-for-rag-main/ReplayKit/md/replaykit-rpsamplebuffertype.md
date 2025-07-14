

- ReplayKit
-  RPSampleBufferType 

Enumeration

# RPSampleBufferType

The type of media clip sample being buffered.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 11.0+tvOS 10.0+visionOS 1.0+

``` source
enum RPSampleBufferType
```

## Topics

### Sample Buffer Types

case audioApp

The sample audio that originates from the app.

case audioMic

The sample audio that originates from the microphone.

case video

The sample that contains a video clip.

### Initializers

init?(rawValue: Int)

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Controlling App Recording

func startRecording(handler: (((any Error)?) -> Void)?)

Starts recording the app display.

func stopRecording(handler: ((RPPreviewViewController?, (any Error)?) -> Void)?)

Stops the current recording.

func stopRecording(withOutput: URL, completionHandler: (((any Error)?) -> Void)?)

Stops the current recording and writes the movie to the specified output URL.

func startCapture(handler: ((CMSampleBuffer, RPSampleBufferType, (any Error)?) -> Void)?, completionHandler: (((any Error)?) -> Void)?)

Starts screen and audio capture.

func stopCapture(handler: (((any Error)?) -> Void)?)

Stops screen capture

func discardRecording(handler: () -> Void)

Discards the current recording.

func startRecording(withMicrophoneEnabled: Bool, handler: (((any Error)?) -> Void)?)

Starts recording the app’s audio and video.

Deprecated

