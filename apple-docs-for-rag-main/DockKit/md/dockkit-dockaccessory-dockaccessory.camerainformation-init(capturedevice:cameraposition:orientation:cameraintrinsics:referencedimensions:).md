

- DockKit
- DockAccessory
- DockAccessory.CameraInformation
-  init(captureDevice:cameraPosition:orientation:cameraIntrinsics:referenceDimensions:) 

Initializer

# init(captureDevice:cameraPosition:orientation:cameraIntrinsics:referenceDimensions:)

Creates an object that describes the camera in use for tracking.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 2.1+

``` source
init(
    captureDevice: AVCaptureDevice.DeviceType,
    cameraPosition: AVCaptureDevice.Position,
    orientation: DockAccessory.CameraOrientation,
    cameraIntrinsics: matrix_float3x3?,
    referenceDimensions: CGSize?
)
```

## Parameters 

`captureDevice`  

The capture device generating the video.

`cameraPosition`  

The physical position of the capture device.

`orientation`  

The orientation of the capture device.

`cameraIntrinsics`  

A matrix that represents the characteristics of the lens.

`referenceDimensions`  

The size of the video frame.

