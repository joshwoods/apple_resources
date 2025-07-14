

- CarPlay
- CPRouteInformation
-  maneuverTravelEstimates 

Instance Property

# maneuverTravelEstimates

An object that describes the time and distance estimates for a maneuver.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+

``` source
@NSCopying
var maneuverTravelEstimates: CPTravelEstimates { get }
```

### Discussion

This is the first maneuver in the current list of maneuvers.

## See Also

### Properties

var currentLaneGuidance: CPLaneGuidance

A lane guidance object that describes the current lane guidance.

var currentManeuvers: [CPManeuver]

An array of maneuver objects that describes the current maneuvers.

var laneGuidances: [CPLaneGuidance]

An array of lane guidance objects.

var maneuvers: [CPManeuver]

An array of maneuver objects.

var tripTravelEstimates: CPTravelEstimates

A travel estimates object that describes the estimated time and distance for the current trip.

