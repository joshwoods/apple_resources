

- CarPlay
- CPNavigationSession
-  currentLaneGuidance 

Instance Property

# currentLaneGuidance

The current lane guidance to use for navigation metadata.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+

``` source
@NSCopying
var currentLaneGuidance: CPLaneGuidance? { get set }
```

## Discussion

First, add the required CPLaneGuidance objects to the session using add(_:), then set this property with the current lane guidance.

Set this property to `nil` if there’s no current lane guidance.

## See Also

### Managing Upcoming Maneuvers

var upcomingManeuvers: [CPManeuver]

The next set of maneuvers the user should perform while following the current route.

var maneuverState: CPManeuverState

The current maneuver state.

var currentRoadNameVariants: [String]

An array of strings that describe variants of the current road name.

func add([CPManeuver])

Adds one or more maneuvers, in chronological order, to the navigation session.

func add([CPLaneGuidance])

Adds one or more lane guidance instances to the navigation session.

class CPManeuver

An object that describes a single navigation instruction.

