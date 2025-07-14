

- CarPlay
- CPNavigationSession
-  pauseTrip(for:description:) 

Instance Method

# pauseTrip(for:description:)

Tells the navigation session to pause the trip for the specified reason.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
func pauseTrip(
    for reason: CPNavigationSession.PauseReason,
    description: String?
)
```

## Parameters 

`reason`  

The reason for pausing the trip.

`description`  

An optional description of the pause reason. To use a system-provided value, set this parameter to `nil`.

## See Also

### Managing Trip Navigation

func cancelTrip()

Tells the navigation session to cancel the trip.

func finishTrip()

Tells the navigation session to finish the trip.

func pauseTrip(for: CPNavigationSession.PauseReason, description: String?, turnCardColor: UIColor?)

enum PauseReason

A set of reasons for pausing a trip.

func resumeTrip(updatedRouteInformation: CPRouteInformation)

Resumes the current trip with updated route information.

