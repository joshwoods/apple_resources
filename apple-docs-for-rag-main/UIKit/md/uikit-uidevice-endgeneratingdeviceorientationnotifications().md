

- UIKit
- UIDevice
-  endGeneratingDeviceOrientationNotifications() 

Instance Method

# endGeneratingDeviceOrientationNotifications()

Ends the generation of notifications of device orientation changes.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+

``` source
@MainActor
func endGeneratingDeviceOrientationNotifications()
```

## Discussion

This method stops the posting of orientationDidChangeNotification notifications and notifies the system that it can power down the accelerometer hardware if it isn’t in use elsewhere. You call this method after a previous call to the beginGeneratingDeviceOrientationNotifications() method.

## See Also

### Tracking the device orientation

var orientation: UIDeviceOrientation

The physical orientation of the device.

enum UIDeviceOrientation

Constants that describe the physical orientation of the device.

var isGeneratingDeviceOrientationNotifications: Bool

A Boolean value that indicates whether the device generates orientation notifications.

func beginGeneratingDeviceOrientationNotifications()

Begins the generation of notifications of device orientation changes.

