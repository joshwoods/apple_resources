

- Core Location
- CLLocationManagerDelegate
-  locationManager(\_:didRange:satisfying:) 

Instance Method

# locationManager(\_:didRange:satisfying:)

Tells the delegate that the location manager detected at least one beacon that satisfies the provided constraint.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+

``` source
optional func locationManager(
    _ manager: CLLocationManager,
    didRange beacons: [CLBeacon],
    satisfying beaconConstraint: CLBeaconIdentityConstraint
)
```

## Parameters 

`manager`  

The CLLocationManager that corresponds to this delegate.

`beacons`  

An array of CLBeacon objects.

`beaconConstraint`  

The CLBeaconIdentityConstraint that describes the characteristics of the beacons the location manager is looking for.

## See Also

### Receiving beacon-related updates

func locationManager(CLLocationManager, didFailRangingFor: CLBeaconIdentityConstraint, error: any Error)

Tells the delegate that the location manager couldn’t detect any beacons that satisfy the provided constraint.

func locationManager(CLLocationManager, didRangeBeacons: [CLBeacon], in: CLBeaconRegion)

Tells the delegate that one or more beacons are in range.

Deprecated

func locationManager(CLLocationManager, rangingBeaconsDidFailFor: CLBeaconRegion, withError: any Error)

Tells the delegate that an error occurred while gathering ranging information for a set of beacons.

Deprecated

