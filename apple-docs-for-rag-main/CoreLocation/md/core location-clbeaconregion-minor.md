

- Core Location
- CLBeaconRegion
-  minor 

Instance Property

# minor

The minor value from the beacon identity constraint that defines the beacon region.

iOS 7.0–18.4DeprecatediPadOS 7.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.15–11.0Deprecated

``` source
@NSCopying
var minor: NSNumber? { get }
```

## Discussion

If you don’t specify a `minor` value for the beacon, the value of this property is `nil`. Operations that compare a beacon’s identity characteristics with the constraint’s characteristics ignore the `minor` value if this property is `nil`.

## See Also

### Getting the beacon identity

var uuid: UUID

The UUID value from the beacon identity constraint that defines the beacon region.

var major: NSNumber?

The major value from the beacon identity constraint that defines the beacon region.

var beaconIdentityConstraint: CLBeaconIdentityConstraint

The beacon identity constraint that defines the beacon region.

