

- CarPlay
- CPNavigationSession
-  currentRoadNameVariants 

Instance Property

# currentRoadNameVariants

An array of strings that describe variants of the current road name.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+

``` source
var currentRoadNameVariants: [String] { get set }
```

## Discussion

Set this property with variants of the current road name, from most to least verbose.

## See Also

### Managing Upcoming Maneuvers

var upcomingManeuvers: [CPManeuver]

The next set of maneuvers the user should perform while following the current route.

var maneuverState: CPManeuverState

The current maneuver state.

var currentLaneGuidance: CPLaneGuidance?

The current lane guidance to use for navigation metadata.

func add([CPManeuver])

Adds one or more maneuvers, in chronological order, to the navigation session.

func add([CPLaneGuidance])

Adds one or more lane guidance instances to the navigation session.

class CPManeuver

An object that describes a single navigation instruction.

