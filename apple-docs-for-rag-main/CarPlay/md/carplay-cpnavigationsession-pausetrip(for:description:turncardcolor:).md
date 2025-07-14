

- CarPlay
- CPNavigationSession
-  pauseTrip(for:description:turnCardColor:) 

Instance Method

# pauseTrip(for:description:turnCardColor:)

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+

``` source
func pauseTrip(
    for reason: CPNavigationSession.PauseReason,
    description: String?,
    turnCardColor: UIColor?
)
```

## See Also

### Managing Trip Navigation

func cancelTrip()

Tells the navigation session to cancel the trip.

func finishTrip()

Tells the navigation session to finish the trip.

func pauseTrip(for: CPNavigationSession.PauseReason, description: String?)

Tells the navigation session to pause the trip for the specified reason.

enum PauseReason

A set of reasons for pausing a trip.

func resumeTrip(updatedRouteInformation: CPRouteInformation)

Resumes the current trip with updated route information.

