

- HomeKit
- HMCameraStreamControlDelegate
-  cameraStreamControlDidStartStream(\_:) 

Instance Method

# cameraStreamControlDidStartStream(\_:)

Tells the delegate that the camera stream has started.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
optional func cameraStreamControlDidStartStream(_ cameraStreamControl: HMCameraStreamControl)
```

## Parameters 

`cameraStreamControl`  

The stream control responsible for the camera stream.

## See Also

### Observing stream activity

func cameraStreamControl(HMCameraStreamControl, didStopStreamWithError: (any Error)?)

Tells the delegate that the camera stream has stopped.

