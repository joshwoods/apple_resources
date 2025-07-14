

- AVFoundation
- AVCaptureDevice
-  isContinuityCamera 

Instance Property

# isContinuityCamera

A Boolean value that indicates whether the device is a Continuity Camera.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 17.0+

``` source
var isContinuityCamera: Bool { get }
```

## Discussion

Continuity Camera enables you to use the rear camera system of iPhone as an external webcam in macOS.

## See Also

### Supporting Continuity Camera

class var systemPreferredCamera: AVCaptureDevice?

A camera the system prefers to use for video and photo capture.

class var userPreferredCamera: AVCaptureDevice?

A camera the user prefers to use for video and photo capture.

var companionDeskViewCamera: AVCaptureDevice?

A Desk View camera associated with a device.

