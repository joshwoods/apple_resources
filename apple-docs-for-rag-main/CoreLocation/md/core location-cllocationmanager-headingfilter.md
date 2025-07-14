

- Core Location
- CLLocationManager
-  headingFilter 

Instance Property

# headingFilter

The minimum angular change in degrees required to generate new heading events.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.15+watchOS 2.0+

``` source
var headingFilter: CLLocationDegrees { get set }
```

## Discussion

The angular distance is measured relative to the last delivered heading event. Use the value kCLHeadingFilterNone to be notified of all movements. The default value of this property is `1` degree.

## See Also

### Running the heading service

func startUpdatingHeading()

Starts the generation of updates that report the user’s current heading.

func stopUpdatingHeading()

Stops the generation of heading updates.

func dismissHeadingCalibrationDisplay()

Dismisses the heading calibration view from the screen immediately.

let kCLHeadingFilterNone: CLLocationDegrees

A constant indicating that all header values should be reported.

typealias CLLocationDegrees

A latitude or longitude value specified in degrees.

var headingOrientation: CLDeviceOrientation

The device orientation to use when computing heading values.

enum CLDeviceOrientation

Constants indicating the physical orientation of the device.

