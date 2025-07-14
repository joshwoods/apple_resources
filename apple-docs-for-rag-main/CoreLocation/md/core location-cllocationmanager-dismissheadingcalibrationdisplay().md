

- Core Location
- CLLocationManager
-  dismissHeadingCalibrationDisplay() 

Instance Method

# dismissHeadingCalibrationDisplay()

Dismisses the heading calibration view from the screen immediately.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.15+watchOS 2.0+

``` source
func dismissHeadingCalibrationDisplay()
```

## Discussion

Core Location uses the heading calibration alert to calibrate the available heading hardware as needed. The display of this view is automatic, assuming your delegate supports displaying the view at all. If the view is displayed, you can use this method to dismiss it after an appropriate amount of time to ensure that your app’s user interface is not unduly disrupted.

## See Also

### Running the heading service

func startUpdatingHeading()

Starts the generation of updates that report the user’s current heading.

func stopUpdatingHeading()

Stops the generation of heading updates.

var headingFilter: CLLocationDegrees

The minimum angular change in degrees required to generate new heading events.

let kCLHeadingFilterNone: CLLocationDegrees

A constant indicating that all header values should be reported.

typealias CLLocationDegrees

A latitude or longitude value specified in degrees.

var headingOrientation: CLDeviceOrientation

The device orientation to use when computing heading values.

enum CLDeviceOrientation

Constants indicating the physical orientation of the device.

