

- Core Location
- CLLocationManagerDelegate
-  locationManager(\_:rangingBeaconsDidFailFor:withError:) Deprecated

Instance Method

# locationManager(\_:rangingBeaconsDidFailFor:withError:)

Tells the delegate that an error occurred while gathering ranging information for a set of beacons.

iOS 7.0–13.0DeprecatediPadOS 7.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.15–10.15Deprecated

``` source
optional func locationManager(
    _ manager: CLLocationManager,
    rangingBeaconsDidFailFor region: CLBeaconRegion,
    withError error: any Error
)
```

Deprecated

Use locationManager(_:didFailRangingFor:error:) instead.

## Parameters 

`manager`  

The location manager object reporting the event.

`region`  

The region object that encountered the error.

`error`  

An error object containing the error code that indicates why ranging failed.

## Discussion

Errors occur most often when registering a beacon region failed. If the region object itself is invalid or if it contains invalid data, the location manager calls this method to report the problem.

## See Also

### Receiving beacon-related updates

func locationManager(CLLocationManager, didRange: [CLBeacon], satisfying: CLBeaconIdentityConstraint)

Tells the delegate that the location manager detected at least one beacon that satisfies the provided constraint.

func locationManager(CLLocationManager, didFailRangingFor: CLBeaconIdentityConstraint, error: any Error)

Tells the delegate that the location manager couldn’t detect any beacons that satisfy the provided constraint.

func locationManager(CLLocationManager, didRangeBeacons: [CLBeacon], in: CLBeaconRegion)

Tells the delegate that one or more beacons are in range.

Deprecated

