

- UIKit
- UIDevice
-  orientation 

Instance Property

# orientation

The physical orientation of the device.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+

``` source
@MainActor
var orientation: UIDeviceOrientation { get }
```

## Discussion

The value of the property is a constant that indicates the current orientation of the device. This value represents the physical orientation of the device and may be different from the current orientation of your application’s user interface. See UIDeviceOrientation for descriptions of the possible values.

The value of this property always returns 0 unless orientation notifications have been enabled by calling beginGeneratingDeviceOrientationNotifications().

## See Also

### Tracking the device orientation

enum UIDeviceOrientation

Constants that describe the physical orientation of the device.

var isGeneratingDeviceOrientationNotifications: Bool

A Boolean value that indicates whether the device generates orientation notifications.

func beginGeneratingDeviceOrientationNotifications()

Begins the generation of notifications of device orientation changes.

func endGeneratingDeviceOrientationNotifications()

Ends the generation of notifications of device orientation changes.

