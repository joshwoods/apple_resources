

- Core Location
- CLLocationManagerDelegate
-  locationManager(\_:didStartMonitoringFor:) 

Instance Method

# locationManager(\_:didStartMonitoringFor:)

Tells the delegate that a new region is being monitored.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+

``` source
optional func locationManager(
    _ manager: CLLocationManager,
    didStartMonitoringFor region: CLRegion
)
```

## Parameters 

`manager`  

The location manager object reporting the event.

`region`  

The region that is being monitored.

## See Also

### Receiving region-related updates

func locationManager(CLLocationManager, didEnterRegion: CLRegion)

Tells the delegate that the user entered the specified region.

func locationManager(CLLocationManager, didExitRegion: CLRegion)

Tells the delegate that the user left the specified region.

func locationManager(CLLocationManager, didDetermineState: CLRegionState, for: CLRegion)

Tells the delegate about the state of the specified region.

func locationManager(CLLocationManager, monitoringDidFailFor: CLRegion?, withError: any Error)

Tells the delegate that a region monitoring error occurred.

enum CLRegionState

Constants that reflect the relationship of the current location to the region boundaries.

