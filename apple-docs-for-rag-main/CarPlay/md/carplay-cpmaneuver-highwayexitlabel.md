

- CarPlay
- CPManeuver
-  highwayExitLabel 

Instance Property

# highwayExitLabel

A string that describes a highway exit.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+

``` source
var highwayExitLabel: String { get set }
```

## Discussion

Set the label to a string that describes the exit, as in the example:

```
   highwayExitLabel = "Exit 123"

```

## See Also

### Providing maneuver information

var maneuverType: CPManeuverType

A value that represents the type of maneuver.

var roadFollowingManeuverVariants: [String]?

An array of strings that represent the names of the road following this maneuver, arranged from most to least preferred.

var linkedLaneGuidance: CPLaneGuidance

A value that represents lane guidance associated with this maneuver.

var trafficSide: CPTrafficSide

A value that represents which side of the road the traffic drives on.

