

- WatchKit
- WKInterfaceDevice
-  wristLocation 

Instance Property

# wristLocation

The wrist on which the user wears the Apple Watch.

watchOS 3.0+

``` source
var wristLocation: WKInterfaceDeviceWristLocation { get }
```

## Discussion

Users specify the wrist placement during the initial setup of Apple Watch, and this property reflects the information provided by the user.

## See Also

### Reading the Device Settings

var name: String

The name of the device.

var model: String

The model information for the device.

var localizedModel: String

The localized version of the model information.

enum WKInterfaceDeviceWristLocation

Constants indicating the wrist on which the user wears the Apple Watch.

var crownOrientation: WKInterfaceDeviceCrownOrientation

The side on which the crown is positioned.

enum WKInterfaceDeviceCrownOrientation

Constants indicating the crown orientation from the user’s perspective.

var preferredContentSizeCategory: String

The preferred font-sizing option.

