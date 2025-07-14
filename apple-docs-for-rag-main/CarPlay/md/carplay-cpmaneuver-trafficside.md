

- CarPlay
- CPManeuver
-  trafficSide 

Instance Property

# trafficSide

A value that represents which side of the road the traffic drives on.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+

``` source
var trafficSide: CPTrafficSide { get set }
```

## Discussion

One of the CPTrafficSide values that indicates which side of the road traffic drives on; a CPManeuver requires this value.

## See Also

### Providing maneuver information

var maneuverType: CPManeuverType

A value that represents the type of maneuver.

var roadFollowingManeuverVariants: [String]?

An array of strings that represent the names of the road following this maneuver, arranged from most to least preferred.

var linkedLaneGuidance: CPLaneGuidance

A value that represents lane guidance associated with this maneuver.

var highwayExitLabel: String

A string that describes a highway exit.

