

- WatchKit
- WKInterfaceDevice
-  name 

Instance Property

# name

The name of the device.

watchOS 2.0+

``` source
var name: String { get }
```

## Discussion

The default value of this property varies according to the device’s operating system version number:

| OS | Default value | Example |
|----|----|----|
| watchOS 8 and earlier | User-assigned device name | `"Ravi’s Apple Watch Ultra (49mm)"` |
| watchOS 9 and later | Generic device name | `"Apple Watch Ultra (49mm)"` |

In watchOS, the *user-assigned device name* is available in the Settings app under General \> About \> Name. To access the user-assigned device name through this property in watchOS 9 and later, your app must meet certain criteria and be assigned an entitlement. For information, see com.apple.developer.device-information.user-assigned-device-name.

Related Sessions from WWDC22

Session 10096: What’s new in privacy

## See Also

### Reading the Device Settings

var model: String

The model information for the device.

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

