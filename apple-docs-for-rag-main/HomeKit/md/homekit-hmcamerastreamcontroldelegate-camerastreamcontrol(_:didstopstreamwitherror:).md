

- HomeKit
- HMCameraStreamControlDelegate
-  cameraStreamControl(\_:didStopStreamWithError:) 

Instance Method

# cameraStreamControl(\_:didStopStreamWithError:)

Tells the delegate that the camera stream has stopped.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
optional func cameraStreamControl(
    _ cameraStreamControl: HMCameraStreamControl,
    didStopStreamWithError error: (any Error)?
)
```

## Parameters 

`cameraStreamControl`  

The stream control responsible for the camera stream.

`error`  

If the stream stops because of an error, this is an error object with details; `nil` otherwise.

## See Also

### Observing stream activity

func cameraStreamControlDidStartStream(HMCameraStreamControl)

Tells the delegate that the camera stream has started.

