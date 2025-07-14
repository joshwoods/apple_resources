

- Core Location
- CLBeaconIdentityConstraint
-  major 

Instance Property

# major

The constraint’s value for the major identity characteristic.

iOS 13.0+iPadOS 13.0+macOS 10.15+

``` source
var major: UInt16? { get }
```

## Discussion

The major characteristic is optional. If it’s present, a beacon’s major value needs to match the constraint’s major value to represent a match. If the constraint has no major value, it acts as a wildcard and matches any major value. You can specify the major value when initializing the constraint.

## See Also

### Getting the beacon identity

var minor: UInt16?

The constraint’s value for the minor identity characteristic.

