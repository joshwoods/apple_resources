

- DockKit
- DockAccessory
-  track(\_:cameraInformation:image:) 

Instance Method

# track(\_:cameraInformation:image:)

Automatically generate and send tracking vectors to the device.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 2.1+

``` source
final func track(
    _ metadata: [AVMetadataObject],
    cameraInformation: DockAccessory.CameraInformation,
    image: CVPixelBuffer
) async throws
```

## Parameters 

`metadata`  

An array of AVMetadataObject objects indicating the location of objects within the frame.

`cameraInformation`  

The camera in current use and its orientation.

`image`  

The captured camera image buffer.

## Discussion

The vectors are based on metadata coming from the camera.

Disable system tracking, then supply the observations at a fixed rate between 10 and 30 times per second. Any other rate is unsupported.

Throws

DockKitError.notSupported if called on macOS.

