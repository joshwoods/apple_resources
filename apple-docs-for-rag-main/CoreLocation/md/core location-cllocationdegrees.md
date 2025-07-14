

- Core Location
-  CLLocationDegrees 

Type Alias

# CLLocationDegrees

A latitude or longitude value specified in degrees.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
typealias CLLocationDegrees = Double
```

## See Also

### Running the heading service

func startUpdatingHeading()

Starts the generation of updates that report the user’s current heading.

func stopUpdatingHeading()

Stops the generation of heading updates.

func dismissHeadingCalibrationDisplay()

Dismisses the heading calibration view from the screen immediately.

var headingFilter: CLLocationDegrees

The minimum angular change in degrees required to generate new heading events.

let kCLHeadingFilterNone: CLLocationDegrees

A constant indicating that all header values should be reported.

var headingOrientation: CLDeviceOrientation

The device orientation to use when computing heading values.

enum CLDeviceOrientation

Constants indicating the physical orientation of the device.

