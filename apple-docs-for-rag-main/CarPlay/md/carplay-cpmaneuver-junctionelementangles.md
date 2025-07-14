

- CarPlay
- CPManeuver
-  junctionElementAngles 

Instance Property

# junctionElementAngles

A set of angles for the rest of the roads of this junction.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+

``` source
var junctionElementAngles: Set>? { get set }
```

### Discussion

This must not include `junctionExitAngle`.

## See Also

### Providing junction information

var junctionType: CPJunctionType

A value that represents the type of junction associated with this maneuver.

var junctionExitAngle: Measurement&lt;UnitAngle>?

The angle of the exit road of this junction.

