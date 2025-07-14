

- Core Location
- CLLocationManagerDelegate
-  locationManager(\_:didUpdateTo:from:) 

Instance Method

# locationManager(\_:didUpdateTo:from:)

Tells the delegate that a new location value is available.

macOS 10.6+

``` source
optional func locationManager(
    _ manager: CLLocationManager,
    didUpdateTo newLocation: CLLocation,
    from oldLocation: CLLocation
)
```

## Parameters 

`manager`  

The location manager object that generated the update event.

`newLocation`  

The new location data.

`oldLocation`  

The location data from the previous update. If this is the first update event delivered by this location manager, this parameter is `nil`.

## Discussion

By the time this message is delivered to your delegate, the new location data is also available directly from the CLLocationManager object. The `newLocation` parameter may contain the data that was cached from a previous usage of the location service. You can use the timestamp property of the location object to determine how recent the location data is.

## See Also

### Receiving location updates

func locationManager(CLLocationManager, didUpdateLocations: [CLLocation])

Tells the delegate that new location data is available.

func locationManager(CLLocationManager, didFinishDeferredUpdatesWithError: (any Error)?)

Tells the delegate that updates will no longer be deferred.

