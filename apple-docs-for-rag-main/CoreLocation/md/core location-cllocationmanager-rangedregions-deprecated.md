

- Core Location
- CLLocationManager
-  rangedRegions Deprecated

Instance Property

# rangedRegions

The set of regions currently being tracked using ranging.

iOS 7.0–13.0DeprecatediPadOS 7.0–13.0DeprecatedMac Catalyst 14.0–14.0DeprecatedmacOS 10.15–10.15Deprecated

``` source
var rangedRegions: Set { get }
```

Deprecated

Use rangedBeaconConstraints instead.

## Discussion

The objects in the set are instances of the CLBeaconRegion class.

## Topics

### Related Documentation

func startRangingBeacons(in: CLBeaconRegion)

Starts the delivery of notifications for the specified beacon region.

## See Also

### Properties

var headingAvailable: Bool

A Boolean value indicating whether the location manager is able to generate heading-related events.

Deprecated

var locationServicesEnabled: Bool

A Boolean value indicating whether location services are enabled on the device.

Deprecated

var purpose: String?

An app-provided string that describes the reason for using location services.

Deprecated

