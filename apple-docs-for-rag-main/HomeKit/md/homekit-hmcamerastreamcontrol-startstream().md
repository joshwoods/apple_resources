

- HomeKit
- HMCameraStreamControl
-  startStream() 

Instance Method

# startStream()

Starts the camera stream.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func startStream()
```

## Discussion

When streaming has successfully started, the cameraStream property is updated with the new stream.

## See Also

### Controlling the stream

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

