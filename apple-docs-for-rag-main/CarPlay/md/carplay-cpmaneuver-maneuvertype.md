

- CarPlay
- CPManeuver
-  maneuverType 

Instance Property

# maneuverType

A value that represents the type of maneuver.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+

``` source
var maneuverType: CPManeuverType { get set }
```

## Discussion

CarPlay requires this value to support route guidance metadata.

## See Also

### Providing maneuver information

var roadFollowingManeuverVariants: [String]?

An array of strings that represent the names of the road following this maneuver, arranged from most to least preferred.

var linkedLaneGuidance: CPLaneGuidance

A value that represents lane guidance associated with this maneuver.

var highwayExitLabel: String

A string that describes a highway exit.

var trafficSide: CPTrafficSide

A value that represents which side of the road the traffic drives on.

