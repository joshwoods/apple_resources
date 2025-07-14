

- Core Location
- CLLocationManager
-  stopRangingBeacons(satisfying:) 

Instance Method

# stopRangingBeacons(satisfying:)

Stops the delivery of notifications for the specified beacon constraints.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+

``` source
func stopRangingBeacons(satisfying constraint: CLBeaconIdentityConstraint)
```

## Parameters 

`constraint`  

A CLBeaconIdentityConstraint constraint.

## See Also

### Performing beacon ranging

func startRangingBeacons(satisfying: CLBeaconIdentityConstraint)

Starts the delivery of notifications for the specified beacon constraints.

var rangedBeaconConstraints: Set&lt;CLBeaconIdentityConstraint>

The set of beacon constraints currently being tracked using ranging.

