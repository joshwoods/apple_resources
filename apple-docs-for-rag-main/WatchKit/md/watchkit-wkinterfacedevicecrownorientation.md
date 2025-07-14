

- WatchKit
-  WKInterfaceDeviceCrownOrientation 

Enumeration

# WKInterfaceDeviceCrownOrientation

Constants indicating the crown orientation from the user’s perspective.

watchOS 3.0+

``` source
enum WKInterfaceDeviceCrownOrientation
```

## Topics

### Constants

case left

The left side of the device.

case right

The right side of the device.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

var crownOrientation: WKInterfaceDeviceCrownOrientation

The side on which the crown is positioned.

var preferredContentSizeCategory: String

The preferred font-sizing option.

