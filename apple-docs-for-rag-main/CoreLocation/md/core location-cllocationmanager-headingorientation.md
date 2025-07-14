

- Core Location
- CLLocationManager
-  headingOrientation 

Instance Property

# headingOrientation

The device orientation to use when computing heading values.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.15+watchOS 2.0+

``` source
var headingOrientation: CLDeviceOrientation { get set }
```

## Mentioned in 

Getting heading and course information

## Discussion

When computing heading values, the location manager assumes that the top of the device in portrait mode represents due north (0 degrees) by default. For apps that run in other orientations, this may not always be the most convenient orientation. This property allows you to specify which device orientation you want the location manager to use as the reference point for due north.

Although you can set the value of this property to CLDeviceOrientation.unknown, CLDeviceOrientation.faceUp, or CLDeviceOrientation.faceDown, doing so has no effect on the orientation reference point. The original reference point is retained instead.

Changing the value in this property affects only those heading values reported after the change is made.

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

typealias CLLocationDegrees

A latitude or longitude value specified in degrees.

enum CLDeviceOrientation

Constants indicating the physical orientation of the device.

