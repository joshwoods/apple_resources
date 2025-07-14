

- CarPlay
- CPRouteInformation
-  init(maneuvers:laneGuidances:currentManeuvers:currentLaneGuidance:trip:maneuverTravelEstimates:) 

Initializer

# init(maneuvers:laneGuidances:currentManeuvers:currentLaneGuidance:trip:maneuverTravelEstimates:)

Initializes a new route information object with maneuvers, lane guidances, the current maneuvers, the current lane guidance, and trip and current maneuver travel estimates.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+

``` source
init(
    maneuvers: [CPManeuver],
    laneGuidances: [CPLaneGuidance],
    currentManeuvers: [CPManeuver],
    currentLaneGuidance: CPLaneGuidance,
    trip tripTravelEstimates: CPTravelEstimates,
    maneuverTravelEstimates: CPTravelEstimates
)
```

## Parameters 

`maneuvers`  

An array of CPManeuver objects.

`laneGuidances`  

An array of CPLaneGuidance objects.

`currentManeuvers`  

An array of `CPManeuver` objects that represent the current list of maneuvers.

`currentLaneGuidance`  

A CPLaneGuidance object that represents the guidance for the current lane.

`maneuverTravelEstimates`  

The `CPTravelEstimates` that present the estimates for the trip’s maneuvers.

