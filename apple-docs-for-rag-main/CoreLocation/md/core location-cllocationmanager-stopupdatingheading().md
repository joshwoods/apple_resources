

- Core Location
- CLLocationManager
-  stopUpdatingHeading() 

Instance Method

# stopUpdatingHeading()

Stops the generation of heading updates.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+watchOS 2.0+

``` source
func stopUpdatingHeading()
```

## Discussion

Call this method whenever your code no longer needs to receive heading-related events. Disabling event delivery gives the receiver the option of disabling the appropriate hardware (and thereby saving power) when no clients need location data. You can always restart the generation of heading updates by calling the startUpdatingHeading() method again.

If a compatible iPad or iPhone app calls this method when running in visionOS, the method does nothing.

## See Also

### Running the heading service

func startUpdatingHeading()

Starts the generation of updates that report the user’s current heading.

func dismissHeadingCalibrationDisplay()

Dismisses the heading calibration view from the screen immediately.

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

