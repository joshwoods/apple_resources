

- Group Activities
- GroupSession
- GroupSession.State
-  GroupSession.State.invalidated(reason:) 

Case

# GroupSession.State.invalidated(reason:)

A state that indicates the session is no longer valid and can’t be used for shared activities.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
case invalidated(reason: any Error)
```

## Mentioned in 

Joining and managing a shared activity

## Discussion

The session transitions to this state when an error occurs, when the FaceTime call ends, or when your app calls the leave() method. When a session is in this state, don’t attempt to join, leave, or end the session again. Instead, release resources related to the session, including the session object itself.

## See Also

### Session states

case waiting

An idle state that indicates the session is waiting for the app to join the activity.

case joined

An active state that indicates the session allows data synchronization between devices.

