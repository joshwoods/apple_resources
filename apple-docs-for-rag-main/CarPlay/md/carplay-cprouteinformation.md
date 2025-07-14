

- CarPlay
-  CPRouteInformation 

Class

# CPRouteInformation

A class that describes the characteristic elements of a route.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+

``` source
class CPRouteInformation
```

## Topics

### Initializers

init(maneuvers: [CPManeuver], laneGuidances: [CPLaneGuidance], currentManeuvers: [CPManeuver], currentLaneGuidance: CPLaneGuidance, trip: CPTravelEstimates, maneuverTravelEstimates: CPTravelEstimates)

Initializes a new route information object with maneuvers, lane guidances, the current maneuvers, the current lane guidance, and trip and current maneuver travel estimates.

### Properties

var currentLaneGuidance: CPLaneGuidance

A lane guidance object that describes the current lane guidance.

var currentManeuvers: [CPManeuver]

An array of maneuver objects that describes the current maneuvers.

var laneGuidances: [CPLaneGuidance]

An array of lane guidance objects.

var maneuverTravelEstimates: CPTravelEstimates

An object that describes the time and distance estimates for a maneuver.

var maneuvers: [CPManeuver]

An array of maneuver objects.

var tripTravelEstimates: CPTravelEstimates

A travel estimates object that describes the estimated time and distance for the current trip.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Routes, lanes and junctions

class CPLane

A class that describes characteristics of a lane on a roadway.

class CPLaneGuidance

A class that provides information that describes the number of lanes on a roadway and navigation instruction variants.

enum CPLaneStatus

Values that describe the status or preferability of a lane.

enum CPJunctionType

Values that represent types of roadway junctions.

