

- UIKit
- UIDevice
-  beginGeneratingDeviceOrientationNotifications() 

Instance Method

# beginGeneratingDeviceOrientationNotifications()

Begins the generation of notifications of device orientation changes.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+

``` source
@MainActor
func beginGeneratingDeviceOrientationNotifications()
```

## Discussion

You must call this method before attempting to get orientation data from the device. This method enables the device’s accelerometer hardware and begins the delivery of acceleration events to the device. The device subsequently uses these events to post orientationDidChangeNotification notifications when the device orientation changes and to update the orientation property.

You may nest calls to this method safely, but you should always match each call with a corresponding call to the endGeneratingDeviceOrientationNotifications() method.

## See Also

### Tracking the device orientation

var orientation: UIDeviceOrientation

The physical orientation of the device.

enum UIDeviceOrientation

Constants that describe the physical orientation of the device.

var isGeneratingDeviceOrientationNotifications: Bool

A Boolean value that indicates whether the device generates orientation notifications.

func endGeneratingDeviceOrientationNotifications()

Ends the generation of notifications of device orientation changes.

