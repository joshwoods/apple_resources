

- Core Location
- CLBeaconRegion
-  uuid 

Instance Property

# uuid

The UUID value from the beacon identity constraint that defines the beacon region.

iOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.15–11.0Deprecated

``` source
var uuid: UUID { get }
```

## Discussion

Typically, the UUID is unique to your company and is the same for all of the beacons that you install. Use the major and minor values to differentiate the beacons in your installation.

## See Also

### Getting the beacon identity

var major: NSNumber?

The major value from the beacon identity constraint that defines the beacon region.

var minor: NSNumber?

The minor value from the beacon identity constraint that defines the beacon region.

var beaconIdentityConstraint: CLBeaconIdentityConstraint

The beacon identity constraint that defines the beacon region.

