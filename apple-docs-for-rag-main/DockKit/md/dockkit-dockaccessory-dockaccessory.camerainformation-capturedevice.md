

- DockKit
- DockAccessory
- DockAccessory.CameraInformation
-  captureDevice 

Instance Property

# captureDevice

The capture device generating the video.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 2.1+

``` source
let captureDevice: AVCaptureDevice.DeviceType
```

## See Also

### Getting camera information

let cameraPosition: AVCaptureDevice.Position

The physical position of the capture device.

let cameraIntrinsics: matrix_float3x3?

A matrix that represents the characteristics of the lens.

let orientation: DockAccessory.CameraOrientation

The orientation of the capture device.

let referenceDimensions: CGSize?

The size of the video frame.

