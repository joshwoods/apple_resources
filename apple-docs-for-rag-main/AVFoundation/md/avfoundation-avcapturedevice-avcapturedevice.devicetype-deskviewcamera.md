

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.DeviceType
-  deskViewCamera 

Type Property

# deskViewCamera

A virtual overhead camera that captures a user’s desk.

macOS 13.0+

``` source
static let deskViewCamera: AVCaptureDevice.DeviceType
```

## Discussion

This device type provides a distortion-corrected cut out from an ultra wide camera that approximates an overhead view of a user’s physical desktop.

You can use this device type with AVCaptureMultiCamSession.

