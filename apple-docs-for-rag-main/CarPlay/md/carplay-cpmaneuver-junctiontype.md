

- CarPlay
- CPManeuver
-  junctionType 

Instance Property

# junctionType

A value that represents the type of junction associated with this maneuver.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+

``` source
var junctionType: CPJunctionType { get set }
```

## Discussion

One of the CPJunctionType values that indicates the type of traffic junction; a CPManeuver requires this value.

## See Also

### Providing junction information

var junctionExitAngle: Measurement&lt;UnitAngle>?

The angle of the exit road of this junction.

var junctionElementAngles: Set&lt;Measurement&lt;UnitAngle>>?

A set of angles for the rest of the roads of this junction.

