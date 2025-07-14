

- XCUIAutomation
- XCUIDevice
-  orientation 

Instance Property

# orientation

The orientation of the device.

iOSiPadOSMac CatalystXcode 16.3+

``` source
@MainActor
var orientation: UIDeviceOrientation { get set }
```

## Discussion

To simulate a change in the physical orientation of a device under test, set the value of the orientation property for the shared XCUIDevice object to one of the UIDeviceOrientation constants UIKit defines. This impacts the orientation property UIKit uses to identify a device’s physical orientation. These constants aren’t tied directly to the orientation of your app’s user interface. The example below sets the device orientation to landscape right:

```
XCUIDevice.shared.orientation = .landscapeRight
```

Set the property once in your test fixture’s setup or intialization code to set an orientation for all the test methods in that fixture.

Available in iOS.

## See Also

### Rotating and changing location

var location: XCUILocation?

The proxy location a test uses to simulate longitude, latitude, and course information for the device.

class XCUILocation

A proxy that simulates a device’s location in terms of its longitude, latitude, and course information.

