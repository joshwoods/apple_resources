

- XCUIAutomation
- XCUILocation
-  location 

Instance Property

# location

Returns the object that contains the latitude, longitude, and course information this proxy simulates for the device.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

``` source
@NSCopying @MainActor
var location: CLLocation { get }
```

## Discussion

Use this property to access the underlying CLLocation this object wraps.

## See Also

### Determining the location

var debugDescription: String

A textual description of the location suitable for debugging.

