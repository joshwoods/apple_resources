

- Core Location
- CLBeaconRegion
-  major 

Instance Property

# major

The major value from the beacon identity constraint that defines the beacon region.

iOS 7.0–18.4DeprecatediPadOS 7.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.15–11.0Deprecated

``` source
@NSCopying
var major: NSNumber? { get }
```

## Discussion

If you don’t specify a major value for the beacon, the value of this property is `nil`. Operations that compare a beacon’s identity characteristics with the constraint’s characteristics ignore the `major` value if this property is `nil`.

## See Also

### Getting the beacon identity

var uuid: UUID

The UUID value from the beacon identity constraint that defines the beacon region.

var minor: NSNumber?

The minor value from the beacon identity constraint that defines the beacon region.

var beaconIdentityConstraint: CLBeaconIdentityConstraint

The beacon identity constraint that defines the beacon region.

