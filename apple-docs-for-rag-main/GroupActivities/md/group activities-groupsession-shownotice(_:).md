

- Group Activities
- GroupSession
-  showNotice(\_:) 

Instance Method

# showNotice(\_:)

Posts an event to the system, which displays the information in the system UI.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
final func showNotice(_ event: GroupSessionEvent)
```

Available when `ActivityType` conforms to `GroupActivity`.

## Parameters 

`event`  

The event to display in the system UI.

## Discussion

Call this method to update the system’s UI with information about session-related events. For example, a music-listening app might post an event to notify the group that a participant stopped playback. The system displays the event information only on the current device, and doesn’t forward events to other devices.

## See Also

### Notifying participants of playback changes

struct GroupSessionEvent

A session-related event that appears in the system UI.

