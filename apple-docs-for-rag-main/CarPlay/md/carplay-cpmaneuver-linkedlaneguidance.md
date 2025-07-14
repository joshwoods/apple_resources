

- CarPlay
- CPManeuver
-  linkedLaneGuidance 

Instance Property

# linkedLaneGuidance

A value that represents lane guidance associated with this maneuver.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+

``` source
unowned(unsafe) var linkedLaneGuidance: CPLaneGuidance { get set }
```

## Discussion

This value is optional; however CPManeuver requires this value if there is a corresponding lane guidance value.

## See Also

### Providing maneuver information

var maneuverType: CPManeuverType

A value that represents the type of maneuver.

var roadFollowingManeuverVariants: [String]?

An array of strings that represent the names of the road following this maneuver, arranged from most to least preferred.

var highwayExitLabel: String

A string that describes a highway exit.

var trafficSide: CPTrafficSide

A value that represents which side of the road the traffic drives on.

