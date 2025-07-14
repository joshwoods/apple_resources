

- Core Location
- CLBeacon
-  rssi 

Instance Property

# rssi

The received signal strength of the beacon, measured in decibels.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.15+

``` source
var rssi: Int { get }
```

## Discussion

This value is the average signal strength of the samples received since Core Location last reported the range of the beacon to your app.

Use this value for calibrating beacon transmission power.

## See Also

### Determining the distance to the beacon

var proximity: CLProximity

The relative distance to the beacon.

enum CLProximity

Constants that reflect the relative distance to a beacon.

var accuracy: CLLocationAccuracy

The accuracy of the proximity value, measured in meters from the beacon.

