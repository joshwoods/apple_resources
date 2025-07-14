

- Core Location
- CLLocationManager
-  startRangingBeacons(satisfying:) 

Instance Method

# startRangingBeacons(satisfying:)

Starts the delivery of notifications for the specified beacon constraints.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+

``` source
func startRangingBeacons(satisfying constraint: CLBeaconIdentityConstraint)
```

## Parameters 

`constraint`  

A CLBeaconIdentityConstraint constraint.

## See Also

### Performing beacon ranging

func stopRangingBeacons(satisfying: CLBeaconIdentityConstraint)

Stops the delivery of notifications for the specified beacon constraints.

var rangedBeaconConstraints: Set&lt;CLBeaconIdentityConstraint>

The set of beacon constraints currently being tracked using ranging.

