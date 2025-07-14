

- UIKit
- UIDevice
-  isGeneratingDeviceOrientationNotifications 

Instance Property

# isGeneratingDeviceOrientationNotifications

A Boolean value that indicates whether the device generates orientation notifications.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+

``` source
@MainActor
var isGeneratingDeviceOrientationNotifications: Bool { get }
```

## Discussion

If the value of this property is true, the shared UIDevice object posts a orientationDidChangeNotification notification when the device changes orientation. If the value is false, it generates no orientation notifications. Device orientation notifications can only be generated between calls to the beginGeneratingDeviceOrientationNotifications() and endGeneratingDeviceOrientationNotifications() methods.

## See Also

### Tracking the device orientation

var orientation: UIDeviceOrientation

The physical orientation of the device.

enum UIDeviceOrientation

Constants that describe the physical orientation of the device.

func beginGeneratingDeviceOrientationNotifications()

Begins the generation of notifications of device orientation changes.

func endGeneratingDeviceOrientationNotifications()

Ends the generation of notifications of device orientation changes.

