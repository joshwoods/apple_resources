

- WatchKit
- WKInterfaceDevice
-  localizedModel 

Instance Property

# localizedModel

The localized version of the model information.

watchOS 2.0+

``` source
var localizedModel: String { get }
```

## Discussion

This property contains the localized string for the value in the model property.

## See Also

### Reading the Device Settings

var name: String

The name of the device.

var model: String

The model information for the device.

var wristLocation: WKInterfaceDeviceWristLocation

The wrist on which the user wears the Apple Watch.

enum WKInterfaceDeviceWristLocation

Constants indicating the wrist on which the user wears the Apple Watch.

var crownOrientation: WKInterfaceDeviceCrownOrientation

The side on which the crown is positioned.

enum WKInterfaceDeviceCrownOrientation

Constants indicating the crown orientation from the user’s perspective.

var preferredContentSizeCategory: String

The preferred font-sizing option.

