

- HomeKit
-  HMCameraStreamControl 

Class

# HMCameraStreamControl

An object that can start and stop the camera stream and contains the view into which the stream is rendered.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class HMCameraStreamControl
```

## Topics

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

enum HMCameraStreamState

The states associated with a camera stream.

### Observing stream activity

var delegate: (any HMCameraStreamControlDelegate)?

Delegate that receives updates as the camera stream changes.

protocol HMCameraStreamControlDelegate

A protocol that gives the delegate updates on the camera stream.

### Initializers

init()Deprecated

## Relationships

### Inherits From

- HMCameraControl

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Streaming

var streamControl: HMCameraStreamControl?

Controls the camera stream.

