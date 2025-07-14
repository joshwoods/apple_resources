

- CarPlay
- CPNavigationSession
-  maneuverState 

Instance Property

# maneuverState

The current maneuver state.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+

``` source
var maneuverState: CPManeuverState { get set }
```

## Discussion

Set this property with the current CPManeuverState based on how close the maneuver is and whether a person needs to act to execute the maneuver.

## See Also

### Managing Upcoming Maneuvers

var upcomingManeuvers: [CPManeuver]

The next set of maneuvers the user should perform while following the current route.

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

