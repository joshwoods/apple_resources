

- AVFoundation
- AVCaptureDevice
-  userPreferredCamera 

Type Property

# userPreferredCamera

A camera the user prefers to use for video and photo capture.

iOS 17.0+iPadOS 17.0+Mac Catalyst 16.0+macOS 13.0+tvOS 17.0+

``` source
class var userPreferredCamera: AVCaptureDevice? { get set }
```

## Discussion

In addition to being a systemPreferredCamera, you can designate a device as a user-preferred camera. Setting a value for this property allows an app to persist its preference across app launches and system reboots. The system internally maintains a short history of devices, so if a user’s most recently preferred camera isn’t currently connected, it still reports the next best choice.

This property always returns a device that’s present. If no camera is available, this value is `nil`.

Note

Setting the value to `nil` has no effect.

## See Also

### Supporting Continuity Camera

class var systemPreferredCamera: AVCaptureDevice?

A camera the system prefers to use for video and photo capture.

var isContinuityCamera: Bool

A Boolean value that indicates whether the device is a Continuity Camera.

var companionDeskViewCamera: AVCaptureDevice?

A Desk View camera associated with a device.

