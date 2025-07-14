

- DockKit
- DockAccessory
- DockAccessory.CameraInformation
-  orientation 

Instance Property

# orientation

The orientation of the capture device.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 2.1+

``` source
let orientation: DockAccessory.CameraOrientation
```

## See Also

### Getting camera information

let cameraPosition: AVCaptureDevice.Position

The physical position of the capture device.

let cameraIntrinsics: matrix_float3x3?

A matrix that represents the characteristics of the lens.

let captureDevice: AVCaptureDevice.DeviceType

The capture device generating the video.

let referenceDimensions: CGSize?

The size of the video frame.

