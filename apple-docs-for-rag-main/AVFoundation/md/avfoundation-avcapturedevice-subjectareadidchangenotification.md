

- AVFoundation
- AVCaptureDevice
-  subjectAreaDidChangeNotification 

Type Property

# subjectAreaDidChangeNotification

A notification the system posts when a capture device detects a substantial change to the video subject area.

iOS 5.0+iPadOS 5.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
class let subjectAreaDidChangeNotification: NSNotification.Name
```

## Discussion

The system posts this notification only if the device’s isSubjectAreaChangeMonitoringEnabled property value is true.

## See Also

### Configuring Camera Hardware

func lockForConfiguration() throws

Requests exclusive access to configure device hardware properties.

func unlockForConfiguration()

Releases exclusive control over device hardware properties.

var isSubjectAreaChangeMonitoringEnabled: Bool

A Boolean value that indicates whether the device monitors the subject area for changes.

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

