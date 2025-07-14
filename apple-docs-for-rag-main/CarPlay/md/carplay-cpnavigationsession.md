

- CarPlay
-  CPNavigationSession 

Class

# CPNavigationSession

An object that represents an active route guidance session.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
class CPNavigationSession
```

## Overview

To start a navigation session, you call startNavigationSession(for:) on the map template, passing the trip the user selected. The map template’s delegate receives the selected trip via mapTemplate(_:startedTrip:using:).

When calculating the initial set of maneuvers, you set pauseTrip(for:description:) to CPNavigationSession.PauseReason.loading so that CarPlay displays the correct state to the user.

During turn-by-turn guidance, you create CPManeuver objects that contain information about upcoming turns, and then update upcomingManeuvers. Maintain at least one maneuver in the array at all times. You should call updateEstimates(_:for:) regularly to update the remaining time and distance for each maneuver.

When CarPlay pauses, finishes, or cancels route guidance, you must call the corresponding method on the active navigation session.

## Topics

### Getting the Trip

var trip: CPTrip

The trip associated with the navigation session.

class CPTrip

An object that represents a journey between an origin and a destination.

### Managing Trip Navigation

func cancelTrip()

Tells the navigation session to cancel the trip.

func finishTrip()

Tells the navigation session to finish the trip.

func pauseTrip(for: CPNavigationSession.PauseReason, description: String?)

Tells the navigation session to pause the trip for the specified reason.

func pauseTrip(for: CPNavigationSession.PauseReason, description: String?, turnCardColor: UIColor?)

enum PauseReason

A set of reasons for pausing a trip.

func resumeTrip(updatedRouteInformation: CPRouteInformation)

Resumes the current trip with updated route information.

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

func add([CPLaneGuidance])

Adds one or more lane guidance instances to the navigation session.

class CPManeuver

An object that describes a single navigation instruction.

### Updating Travel Estimates

func updateEstimates(CPTravelEstimates, for: CPManeuver)

Updates the travel estimates for the specified maneuver.

class CPTravelEstimates

An object that describes the time and distance remaining for a maneuver in a navigation session.

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

## See Also

### Navigating a Trip

func startNavigationSession(for: CPTrip) -> CPNavigationSession

Begins navigational guidance for a trip.

