

- Group Activities
- GroupSessionEvent
-  action 

Instance Property

# action

The reason for the event.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
let action: GroupSessionEvent.Action
```

## Discussion

The system uses this information to craft a message in the system UI.

## See Also

### Getting the event details

let originator: Participant

The participant that initiated the event.

let url: URL?

The URL to open when the participant taps the event link in the system UI.

struct Action

A playback-related change that occurs during the session.

