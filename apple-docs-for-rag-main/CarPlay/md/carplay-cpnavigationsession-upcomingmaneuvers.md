

- CarPlay
- CPNavigationSession
-  upcomingManeuvers 

Instance Property

# upcomingManeuvers

The next set of maneuvers the user should perform while following the current route.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
var upcomingManeuvers: [CPManeuver] { get set }
```

## Discussion

The system displays multiple maneuvers at the same time. However, the system may limit the number of visible maneuvers.

## See Also

### Managing Upcoming Maneuvers

var maneuverState: CPManeuverState

The current maneuver state.

var currentRoadNameVariants: [String]

An array of strings that describe variants of the current road name.

var currentLaneGuidance: CPLaneGuidance?

The current lane guidance to use for navigation metadata.

func add([CPManeuver])

Adds one or more maneuvers, in chronological order, to the navigation session.

func add([CPLaneGuidance])

Adds one or more lane guidance instances to the navigation session.

class CPManeuver

An object that describes a single navigation instruction.

