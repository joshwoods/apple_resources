

- ARKit
- ARConfiguration
- ARConfiguration.VideoFormat
-  captureDeviceType 

Instance Property

# captureDeviceType

The camera that supplies the video format.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+

``` source
var captureDeviceType: AVCaptureDevice.DeviceType { get }
```

## Discussion

To specify a particular video format, select from your configuration’s supportedVideoFormats and set the desired format to the configuration’s videoFormat property.

For example, to specify the ultra-wide camera in a face-tracking session, search the supported video formats for the builtInUltraWideCamera capture device.

```
let config = ARFaceTrackingConfiguration()
for videoFormat in ARFaceTrackingConfiguration.supportedVideoFormats {
    if videoFormat.captureDeviceType == .builtInUltraWideCamera {
        config.videoFormat = videoFormat
        break
    }
}
session.run(config)
```

Important

AR frames only contain depth data (capturedDepthData) in face-tracking sessions that use the TrueDepth camera.

## See Also

### Inspecting the video source

var captureDevicePosition: AVCaptureDevice.Position

The position of the capture device.

enum AVCaptureDevice.Position

Constants that indicate the physical position of a capture device.

