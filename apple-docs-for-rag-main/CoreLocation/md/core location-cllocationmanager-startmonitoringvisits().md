

- Core Location
- CLLocationManager
-  startMonitoringVisits() 

Instance Method

# startMonitoringVisits()

Starts the delivery of visit-related events.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.15+

``` source
func startMonitoringVisits()
```

## Mentioned in 

Getting the current location of a device

## Discussion

Calling this method begins the delivery of visit-related events to your app. Enabling visit events for one location manager enables visit events for all other location manager objects in your app. When a new visit event arrives, the location manager object delivers the event to the locationManager(_:didVisit:) method of its delegate.

Your app can monitor for visit events without calling `requestTemporaryPreciseLocationAuthorization(withPurposeKey:)`. In that case, the visit events use reduced accuracy, as reflected by the horizontalAccuracy property of CLVisit.

If your app is terminated while this service is active, the system relaunches your app when new visit events are ready to be delivered. Upon relaunch, recreate your location manager object and assign a delegate to begin receiving visit events. You don’t need to call this method again to restart the delivery of visit events, but calling it does no harm.

If a compatible iPad or iPhone app calls this method when running in visionOS, the method does nothing.

## See Also

### Running the visits location service

func stopMonitoringVisits()

Stops the delivery of visit-related events.

