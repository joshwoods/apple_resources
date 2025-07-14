

- Core Location
- CLLocationManager
-  requestLocation() 

Instance Method

# requestLocation()

Requests the one-time delivery of the user’s current location.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.14+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func requestLocation()
```

## Mentioned in 

Getting the current location of a device

## Discussion

This method returns immediately. Calling it causes the location manager to obtain a location fix (which may take several seconds) and call the delegate’s locationManager(_:didUpdateLocations:) method with the result. The location fix is obtained at the accuracy level indicated by the desiredAccuracy property. Only one location fix is reported to the delegate, after which location services are stopped. If a location fix cannot be determined in a timely manner, the location manager calls the delegate’s locationManager(_:didFailWithError:) method instead and reports a CLError.Code.locationUnknown error.

Use this method when you want the user’s current location but do not need to leave location services running. This method starts location services long enough to return a result or report an error and then stops them again. Calling the startUpdatingLocation() or allowDeferredLocationUpdates(untilTraveled:timeout:) method cancels any pending request made using this method. Calling this method while location services are already running does nothing. To cancel a pending request, call the stopUpdatingLocation() method.

If obtaining the desired accuracy would take too long, the location manager delivers a less accurate location value rather than reporting an error.

When using this method, the associated delegate must implement the locationManager(_:didUpdateLocations:) and locationManager(_:didFailWithError:) methods. Failure to do so is a programmer error.

## See Also

### Running the standard location service

func startUpdatingLocation()

Starts the generation of updates that report the user’s current location.

func stopUpdatingLocation()

Stops the generation of location updates.

var pausesLocationUpdatesAutomatically: Bool

A Boolean value that indicates whether the location-manager object may pause location updates.

var allowsBackgroundLocationUpdates: Bool

A Boolean value that indicates whether the app receives location updates when running in the background.

var showsBackgroundLocationIndicator: Bool

A Boolean value that indicates whether the status bar changes its appearance when an app uses location services in the background.

var activityType: CLActivityType

The type of activity the app expects the user to typically perform while in the app’s location session.

enum CLActivityType

Constants that indicate the type of activity associated with location updates.

