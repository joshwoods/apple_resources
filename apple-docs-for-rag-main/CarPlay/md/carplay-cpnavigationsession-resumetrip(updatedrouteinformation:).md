

- CarPlay
- CPNavigationSession
-  resumeTrip(updatedRouteInformation:) 

Instance Method

# resumeTrip(updatedRouteInformation:)

Resumes the current trip with updated route information.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+

``` source
func resumeTrip(updatedRouteInformation routeInformation: CPRouteInformation)
```

## Parameters 

`routeInformation`  

The updated route information for the current trip.

## See Also

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

