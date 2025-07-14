

- CarPlay
- CPNavigationSession
-  CPNavigationSession.PauseReason 

Enumeration

# CPNavigationSession.PauseReason

A set of reasons for pausing a trip.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
enum PauseReason
```

## Topics

### Reasons

case arrived

The user arrived at the destination.

case loading

The system is loading the route.

case locating

The system is locating the destination.

case proceedToRoute

The system is waiting for the user to proceed to the route.

case rerouting

The system is rerouting the trip.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing Trip Navigation

func cancelTrip()

Tells the navigation session to cancel the trip.

func finishTrip()

Tells the navigation session to finish the trip.

func pauseTrip(for: CPNavigationSession.PauseReason, description: String?)

Tells the navigation session to pause the trip for the specified reason.

func pauseTrip(for: CPNavigationSession.PauseReason, description: String?, turnCardColor: UIColor?)

func resumeTrip(updatedRouteInformation: CPRouteInformation)

Resumes the current trip with updated route information.

