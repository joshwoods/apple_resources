

- Core Location
- CLLocationManager
-  startUpdatingHeading() 

Instance Method

# startUpdatingHeading()

Starts the generation of updates that report the user’s current heading.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.15+watchOS 2.0+

``` source
func startUpdatingHeading()
```

## Mentioned in 

Getting heading and course information

## Discussion

This method returns immediately. Calling this method when the receiver is stopped causes it to obtain an initial heading and notify your delegate. After that, the receiver generates update events when the value in the headingFilter property is exceeded.

Before calling this method, you should always check the headingAvailable property to see whether heading information is supported on the current device. If heading information is not supported, calling this method has no effect and does not result in the delivery of events to your delegate.

Calling this method several times in succession does not automatically result in new events being generated. Calling stopUpdatingHeading() in between, however, does cause a new initial event to be sent the next time you call this method.

If you start this service and your app is suspended, the system stops the delivery of events until your app starts running again (either in the foreground or background). If your app is terminated, the delivery of new heading events stops altogether and must be restarted by your code when the app is relaunched.

Heading events are delivered to the locationManager(_:didUpdateHeading:) method of your delegate. If there is an error, the location manager calls the locationManager(_:didFailWithError:) method of your delegate instead.

If a compatible iPad or iPhone app calls this method when running in visionOS, the method does nothing.

## Topics

### Related Documentation

var headingAvailable: Bool

A Boolean value indicating whether the location manager is able to generate heading-related events.

Deprecated

## See Also

### Running the heading service

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

var headingOrientation: CLDeviceOrientation

The device orientation to use when computing heading values.

enum CLDeviceOrientation

Constants indicating the physical orientation of the device.

