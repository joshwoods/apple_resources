

- Core Location
-  CLRegionState 

Enumeration

# CLRegionState

Constants that reflect the relationship of the current location to the region boundaries.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+

``` source
@frozen
enum CLRegionState
```

## Topics

### Region States

case unknown

It is unknown whether the location is inside or outside of the region.

case inside

The location is inside of the given region.

case outside

The location is outside of the given region.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

func locationManager(CLLocationManager, didStartMonitoringFor: CLRegion)

Tells the delegate that a new region is being monitored.

