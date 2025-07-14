

- Core Location
- CLBeacon
-  proximity 

Instance Property

# proximity

The relative distance to the beacon.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.15+

``` source
var proximity: CLProximity { get }
```

## Discussion

The value in this property gives a general sense of the relative distance to the beacon. Use it to quickly identify beacons that are nearer to the user rather than farther away.

## See Also

### Determining the distance to the beacon

enum CLProximity

Constants that reflect the relative distance to a beacon.

var accuracy: CLLocationAccuracy

The accuracy of the proximity value, measured in meters from the beacon.

var rssi: Int

The received signal strength of the beacon, measured in decibels.

