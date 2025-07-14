

- AVFoundation
- AVCaptureDevice
-  lockForConfiguration() 

Instance Method

# lockForConfiguration()

Requests exclusive access to configure device hardware properties.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 1.0+

``` source
func lockForConfiguration() throws
```

## Discussion

To set hardware properties on a capture device, such as the focusMode and exposureMode, your app must first acquire a lock on the device. Only hold the device lock if your app requires settable device properties to remain unchanged. Holding the device lock unnecessarily may degrade capture quality in other apps sharing the device.

## See Also

### Configuring Camera Hardware

func unlockForConfiguration()

Releases exclusive control over device hardware properties.

var isSubjectAreaChangeMonitoringEnabled: Bool

A Boolean value that indicates whether the device monitors the subject area for changes.

class let subjectAreaDidChangeNotification: NSNotification.Name

A notification the system posts when a capture device detects a substantial change to the video subject area.

Formats

Configure capture formats and camera frame rates.

Focus

Configure the automatic focus behavior of a camera, or manually set its lens position.

Exposure

Configure the automatic exposure behavior of a camera, or manually control its exposure settings.

White Balance

Configure the automatic white balance behavior of a camera, or manually control white balance settings.

Lighting

Configure the device flash, torch, and low light settings.

Color

Manage HDR and color space settings for a device.

Zoom

Configure device zooming behavior and inspect hardware capabilities.

