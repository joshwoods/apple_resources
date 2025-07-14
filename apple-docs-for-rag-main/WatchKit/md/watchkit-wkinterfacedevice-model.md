

- WatchKit
- WKInterfaceDevice
-  model 

Instance Property

# model

The model information for the device.

watchOS 2.0+

``` source
var model: String { get }
```

## Discussion

For Apple Watch, the value of this string is `Apple Watch`.

## See Also

### Reading the Device Settings

var name: String

The name of the device.

var localizedModel: String

The localized version of the model information.

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

