

- Core Location
- CLLocationManagerDelegate
-  locationManager(\_:didDetermineState:for:) 

Instance Method

# locationManager(\_:didDetermineState:for:)

Tells the delegate about the state of the specified region.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+

``` source
optional func locationManager(
    _ manager: CLLocationManager,
    didDetermineState state: CLRegionState,
    for region: CLRegion
)
```

## Parameters 

`manager`  

The location manager object reporting the event.

`state`  

The state of the specified region. For a list of possible values, see the CLRegionState type.

`region`  

The region whose state was determined.

## Discussion

The location manager calls this method whenever there is a boundary transition for a region. It calls this method in addition to calling the locationManager(_:didEnterRegion:) and locationManager(_:didExitRegion:) methods. The location manager also calls this method in response to a call to its requestState(for:) method, which runs asynchronously.

## See Also

### Receiving region-related updates

func locationManager(CLLocationManager, didEnterRegion: CLRegion)

Tells the delegate that the user entered the specified region.

func locationManager(CLLocationManager, didExitRegion: CLRegion)

Tells the delegate that the user left the specified region.

func locationManager(CLLocationManager, monitoringDidFailFor: CLRegion?, withError: any Error)

Tells the delegate that a region monitoring error occurred.

func locationManager(CLLocationManager, didStartMonitoringFor: CLRegion)

Tells the delegate that a new region is being monitored.

enum CLRegionState

Constants that reflect the relationship of the current location to the region boundaries.

