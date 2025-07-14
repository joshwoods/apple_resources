

- AVFoundation
- AVCaptureDevice
-  isSubjectAreaChangeMonitoringEnabled 

Instance Property

# isSubjectAreaChangeMonitoringEnabled

A Boolean value that indicates whether the device monitors the subject area for changes.

iOS 5.0+iPadOS 5.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var isSubjectAreaChangeMonitoringEnabled: Bool { get set }
```

## Discussion

The value of this property indicates whether the device monitors the video subject area for changes, such as lighting changes, substantial movement, and so on. If you enable subject area change monitoring, the capture device object sends an subjectAreaDidChangeNotification whenever it detects a change to the subject area. You can observe this notification and take action such as focusing, adjusting exposure, and so on.

Before changing the value of this property, you must call lockForConfiguration() to acquire exclusive access to the device’s configuration properties. Otherwise, setting the value of this property raises an exception. When you’re finished configuring the device, call unlockForConfiguration() to release the lock and allow other devices to configure the settings.

This property is key-value observable.

## See Also

### Configuring Camera Hardware

func lockForConfiguration() throws

Requests exclusive access to configure device hardware properties.

func unlockForConfiguration()

Releases exclusive control over device hardware properties.

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

