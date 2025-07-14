

- HomeKit
-  HMCameraStreamState 

Enumeration

# HMCameraStreamState

The states associated with a camera stream.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
enum HMCameraStreamState
```

## Topics

### Observing the streaming state

case notStreaming

The state when the camera stream is not active.

case starting

The state when the camera stream start request is processing.

case stopping

The state when the camera stream is stopping.

case streaming

The state when the camera stream is currently in progress.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Controlling the stream

func startStream()

Starts the camera stream.

func stopStream()

Stops the camera stream.

var cameraStream: HMCameraStream?

The current camera stream.

class HMCameraStream

An object that represents a camera’s audiovisual stream.

var streamState: HMCameraStreamState

The current state of the camera stream.

