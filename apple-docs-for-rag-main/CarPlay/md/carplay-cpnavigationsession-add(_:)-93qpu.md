

- CarPlay
- CPNavigationSession
-  add(\_:) 

Instance Method

# add(\_:)

Adds one or more lane guidance instances to the navigation session.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+

``` source
func add(_ laneGuidances: [CPLaneGuidance])
```

## Discussion

Use this method to add CPLaneGuidance elements in chronological order to the navigation session. Add CPLaneGuidance objects as soon as they are available.

## See Also

### Managing Upcoming Maneuvers

var upcomingManeuvers: [CPManeuver]

The next set of maneuvers the user should perform while following the current route.

var maneuverState: CPManeuverState

The current maneuver state.

var currentRoadNameVariants: [String]

An array of strings that describe variants of the current road name.

var currentLaneGuidance: CPLaneGuidance?

The current lane guidance to use for navigation metadata.

func add([CPManeuver])

Adds one or more maneuvers, in chronological order, to the navigation session.

class CPManeuver

An object that describes a single navigation instruction.

