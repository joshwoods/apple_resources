

- DockKit
- DockAccessory
-  track(\_:cameraInformation:image:) 

Instance Method

# track(\_:cameraInformation:image:)

Automatically generate and send tracking vectors to the device.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 2.1+

``` source
final func track(
    _ data: [DockAccessory.Observation],
    cameraInformation: DockAccessory.CameraInformation,
    image: CVPixelBuffer
) async throws
```

## Parameters 

`data`  

An array of DockAccessory.Observation objects indicating the location of objects of interest in the frame.

`cameraInformation`  

The camera currently being used, and the orientation of the device.

`image`  

The captured camera image buffer.

## Discussion

The device receives tracking vectors based on manually constructed observations.

Disable system tracking, then supply the observations at a fixed rate between 10 and 30 times per second. Any other rate is unsupported. Calling this method without first disabling system tracking is a fatal error.

Throws

DockKitError.notSupported if called on macOS.

