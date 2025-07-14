

- CarPlay
-  CPTravelEstimates 

Class

# CPTravelEstimates

An object that describes the time and distance remaining for a maneuver in a navigation session.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
class CPTravelEstimates
```

## Topics

### Getting the trip

class CPTrip

An object that represents a journey between an origin and a destination.

### Managing upcoming maneuvers

func add([CPManeuver])

Adds one or more maneuvers, in chronological order, to the navigation session.

func add([CPLaneGuidance])

Adds one or more lane guidance instances to the navigation session.

class CPManeuver

An object that describes a single navigation instruction.

### Creating a Travel Estimates Object

init(distanceRemaining: Measurement&lt;UnitLength>, timeRemaining: TimeInterval)

Creates travel estimates with the remaining distance and time.

init(distanceRemaining: Measurement&lt;UnitLength>, distanceRemainingToDisplay: Measurement&lt;UnitLength>, timeRemaining: TimeInterval)

Creates a travel estimates instance with the distance remaining that the framework displays to a person.

### Updating travel estimates

func updateEstimates(CPTravelEstimates, for: CPManeuver)

Updates the travel estimates for the specified maneuver.

### Managing trip navigation

func cancelTrip()

Tells the navigation session to cancel the trip.

func finishTrip()

Tells the navigation session to finish the trip.

func pauseTrip(for: CPNavigationSession.PauseReason, description: String?)

Tells the navigation session to pause the trip for the specified reason.

func pauseTrip(for: CPNavigationSession.PauseReason, description: String?, turnCardColor: UIColor?)

func resumeTrip(updatedRouteInformation: CPRouteInformation)

Resumes the current trip with updated route information.

enum PauseReason

A set of reasons for pausing a trip.

### Getting Travel Estimates

var distanceRemaining: Measurement&lt;UnitLength>

The remaining distance for the travel estimate.

var distanceRemainingToDisplay: Measurement&lt;UnitLength>

The distance remaining that the framework displays to a person, in the default units of measurement.

var timeRemaining: TimeInterval

The remaining time for the travel estimate.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Updating Travel Estimates

func updateEstimates(CPTravelEstimates, for: CPManeuver)

Updates the travel estimates for the specified maneuver.

