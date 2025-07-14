

- HomeKit
- HMCameraStreamControl
-  cameraStream 

Instance Property

# cameraStream

The current camera stream.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var cameraStream: HMCameraStream? { get }
```

## See Also

### Controlling the stream

func startStream()

Starts the camera stream.

func stopStream()

Stops the camera stream.

class HMCameraStream

An object that represents a camera’s audiovisual stream.

var streamState: HMCameraStreamState

The current state of the camera stream.

enum HMCameraStreamState

The states associated with a camera stream.

