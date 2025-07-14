

- CarPlay
- CPNavigationSession
-  finishTrip() 

Instance Method

# finishTrip()

Tells the navigation session to finish the trip.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
func finishTrip()
```

## See Also

### Managing Trip Navigation

func cancelTrip()

Tells the navigation session to cancel the trip.

func pauseTrip(for: CPNavigationSession.PauseReason, description: String?)

Tells the navigation session to pause the trip for the specified reason.

func pauseTrip(for: CPNavigationSession.PauseReason, description: String?, turnCardColor: UIColor?)

enum PauseReason

A set of reasons for pausing a trip.

func resumeTrip(updatedRouteInformation: CPRouteInformation)

Resumes the current trip with updated route information.

