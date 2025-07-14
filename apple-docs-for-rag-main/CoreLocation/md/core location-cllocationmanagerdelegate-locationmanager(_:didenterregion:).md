

- Core Location
- CLLocationManagerDelegate
-  locationManager(\_:didEnterRegion:) 

Instance Method

# locationManager(\_:didEnterRegion:)

Tells the delegate that the user entered the specified region.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.8+

``` source
optional func locationManager(
    _ manager: CLLocationManager,
    didEnterRegion region: CLRegion
)
```

## Parameters 

`manager`  

The location manager object reporting the event.

`region`  

An object containing information about the region that was entered.

## Mentioned in 

Determining the proximity to an iBeacon device

## Discussion

Because regions are a shared application resource, every active location manager object delivers this message to its associated delegate. It doesn’t matter which location manager actually registered the specified region. If multiple location managers share a delegate object, that delegate receives the message multiple times.

The region object provided may not be the same one that was registered. As a result, you should never perform pointer-level comparisons to determine equality. Instead, use the region’s identifier string to determine if your delegate should respond.

## See Also

### Receiving region-related updates

func locationManager(CLLocationManager, didExitRegion: CLRegion)

Tells the delegate that the user left the specified region.

func locationManager(CLLocationManager, didDetermineState: CLRegionState, for: CLRegion)

Tells the delegate about the state of the specified region.

func locationManager(CLLocationManager, monitoringDidFailFor: CLRegion?, withError: any Error)

Tells the delegate that a region monitoring error occurred.

func locationManager(CLLocationManager, didStartMonitoringFor: CLRegion)

Tells the delegate that a new region is being monitored.

enum CLRegionState

Constants that reflect the relationship of the current location to the region boundaries.

