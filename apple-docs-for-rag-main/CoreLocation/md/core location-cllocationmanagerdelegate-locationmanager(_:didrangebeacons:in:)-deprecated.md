

- Core Location
- CLLocationManagerDelegate
-  locationManager(\_:didRangeBeacons:in:) Deprecated

Instance Method

# locationManager(\_:didRangeBeacons:in:)

Tells the delegate that one or more beacons are in range.

iOS 7.0–13.0DeprecatediPadOS 7.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.15–10.15Deprecated

``` source
optional func locationManager(
    _ manager: CLLocationManager,
    didRangeBeacons beacons: [CLBeacon],
    in region: CLBeaconRegion
)
```

Deprecated

Use locationManager(_:didRange:satisfying:) instead.

## Parameters 

`manager`  

The location manager object reporting the event.

`beacons`  

An array of CLBeacon objects representing the beacons currently in range. If `beacons` is empty, you can assume that no beacons matching the specified region are in range. When a specific beacon is no longer in `beacons`, that beacon is no longer received by the device. You can use the information in the CLBeacon objects to determine the range of each beacon and its identifying information.

`region`  

The region object containing the parameters that were used to locate the beacons.

## Mentioned in 

Determining the proximity to an iBeacon device

## Discussion

The location manager calls this method when a new set of beacons becomes available in the specified region or when a beacon goes out of range. The location manager also calls this method when the range of a beacon changes; for example, when a beacon gets closer.

## See Also

### Receiving beacon-related updates

func locationManager(CLLocationManager, didRange: [CLBeacon], satisfying: CLBeaconIdentityConstraint)

Tells the delegate that the location manager detected at least one beacon that satisfies the provided constraint.

func locationManager(CLLocationManager, didFailRangingFor: CLBeaconIdentityConstraint, error: any Error)

Tells the delegate that the location manager couldn’t detect any beacons that satisfy the provided constraint.

func locationManager(CLLocationManager, rangingBeaconsDidFailFor: CLBeaconRegion, withError: any Error)

Tells the delegate that an error occurred while gathering ranging information for a set of beacons.

Deprecated

