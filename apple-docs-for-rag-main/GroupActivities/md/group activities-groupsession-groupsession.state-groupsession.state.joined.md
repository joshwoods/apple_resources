

- Group Activities
- GroupSession
- GroupSession.State
-  GroupSession.State.joined 

Case

# GroupSession.State.joined

An active state that indicates the session allows data synchronization between devices.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
case joined
```

## Mentioned in 

Joining and managing a shared activity

## Discussion

Call the join() method to begin the transition to this state. When the transition completes, use the session object to synchronize your app’s data with the other participants’ devices.

## See Also

### Session states

case waiting

An idle state that indicates the session is waiting for the app to join the activity.

case invalidated(reason: any Error)

A state that indicates the session is no longer valid and can’t be used for shared activities.

