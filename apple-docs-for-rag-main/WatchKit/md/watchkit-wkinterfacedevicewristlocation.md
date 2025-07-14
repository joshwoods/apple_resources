

- WatchKit
-  WKInterfaceDeviceWristLocation 

Enumeration

# WKInterfaceDeviceWristLocation

Constants indicating the wrist on which the user wears the Apple Watch.

watchOS 3.0+

``` source
enum WKInterfaceDeviceWristLocation
```

## Topics

### Constants

case left

The user’s left wrist.

case right

The user’s right wrist.

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

var crownOrientation: WKInterfaceDeviceCrownOrientation

The side on which the crown is positioned.

enum WKInterfaceDeviceCrownOrientation

Constants indicating the crown orientation from the user’s perspective.

var preferredContentSizeCategory: String

The preferred font-sizing option.

