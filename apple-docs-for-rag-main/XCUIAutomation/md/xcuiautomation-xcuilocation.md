

- XCUIAutomation
-  XCUILocation 

Class

# XCUILocation

A proxy that simulates a device’s location in terms of its longitude, latitude, and course information.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor
class XCUILocation
```

## Topics

### Creating a location

init(location: CLLocation)

Initializes a proxy that simulates latitude, longitude, and course information based on the location object you provide.

### Determining the location

var location: CLLocation

Returns the object that contains the latitude, longitude, and course information this proxy simulates for the device.

var debugDescription: String

A textual description of the location suitable for debugging.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Rotating and changing location

var orientation: UIDeviceOrientation

The orientation of the device.

var location: XCUILocation?

The proxy location a test uses to simulate longitude, latitude, and course information for the device.

