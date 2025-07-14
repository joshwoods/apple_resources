

- Core Location
- CLLocationManager
-  rangedBeaconConstraints 

Instance Property

# rangedBeaconConstraints

The set of beacon constraints currently being tracked using ranging.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+

``` source
var rangedBeaconConstraints: Set { get }
```

## See Also

### Performing beacon ranging

func startRangingBeacons(satisfying: CLBeaconIdentityConstraint)

Starts the delivery of notifications for the specified beacon constraints.

func stopRangingBeacons(satisfying: CLBeaconIdentityConstraint)

Stops the delivery of notifications for the specified beacon constraints.

