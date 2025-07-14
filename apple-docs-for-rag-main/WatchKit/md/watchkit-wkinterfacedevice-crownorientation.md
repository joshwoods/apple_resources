

- WatchKit
- WKInterfaceDevice
-  crownOrientation 

Instance Property

# crownOrientation

The side on which the crown is positioned.

watchOS 3.0+

``` source
var crownOrientation: WKInterfaceDeviceCrownOrientation { get }
```

## Discussion

Users specify the Digital Crown orientation during the initial setup of Apple Watch, and this property reflects the information provided by the user.

## See Also

### Reading the Device Settings

var name: String

The name of the device.

var model: String

The model information for the device.

var localizedModel: String

The localized version of the model information.

var wristLocation: WKInterfaceDeviceWristLocation

The wrist on which the user wears the Apple Watch.

enum WKInterfaceDeviceWristLocation

Constants indicating the wrist on which the user wears the Apple Watch.

enum WKInterfaceDeviceCrownOrientation

Constants indicating the crown orientation from the user’s perspective.

var preferredContentSizeCategory: String

The preferred font-sizing option.

