

- HealthKit
- HKDevice
-  local() 

Type Method

# local()

returns a device object that represents the current device.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
class func local() -> HKDevice
```

## Return Value

A device object representing the hardware (iPhone, iPod Touch, or Apple Watch) that is running the app.

## See Also

### Creating Device Objects

init(name: String?, manufacturer: String?, model: String?, hardwareVersion: String?, firmwareVersion: String?, softwareVersion: String?, localIdentifier: String?, udiDeviceIdentifier: String?)

Initializes a new device object.

