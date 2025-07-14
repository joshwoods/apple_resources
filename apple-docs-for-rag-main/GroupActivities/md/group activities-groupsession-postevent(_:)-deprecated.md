

- Group Activities
- GroupSession
-  postEvent(\_:) Deprecated

Instance Method

# postEvent(\_:)

Posts an event to the system, which displays the information in the system UI.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
final func postEvent(_ event: GroupSession.Event)
```

Available when `ActivityType` conforms to `GroupActivity`.

Deprecated

Use GroupSessionEvent

## Parameters 

`event`  

The event to display in the system UI.

## Discussion

Call this method to update the system’s UI with information about session-related events. For example, a music-listening app might post an event to notify the group that a participant added a song to a shared playlist. The system displays the event information only on the current device. It doesn’t forward events to other devices.

