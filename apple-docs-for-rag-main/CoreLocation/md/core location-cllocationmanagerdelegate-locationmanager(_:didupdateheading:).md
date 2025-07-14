

- Core Location
- CLLocationManagerDelegate
-  locationManager(\_:didUpdateHeading:) 

Instance Method

# locationManager(\_:didUpdateHeading:)

Tells the delegate that the location manager received updated heading information.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.15+watchOS 2.0+

``` source
optional func locationManager(
    _ manager: CLLocationManager,
    didUpdateHeading newHeading: CLHeading
)
```

## Parameters 

`manager`  

The location manager object that generated the update event.

`newHeading`  

The new heading data.

## Mentioned in 

Getting heading and course information

## Discussion

Implementation of this method is optional but expected if you start heading updates using the startUpdatingHeading() method.

The location manager object calls this method after you initially start the heading service. Subsequent events are delivered when the previously reported value changes by more than the value specified in the headingFilter property of the location manager object.

## See Also

### Receiving heading updates

func locationManagerShouldDisplayHeadingCalibration(CLLocationManager) -> Bool

Asks the delegate whether the heading calibration alert should be displayed.

