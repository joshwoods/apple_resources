

- Group Activities
- GroupSessionEvent
- GroupSessionEvent.Action
-  seek 

Type Property

# seek

An event that indicates a change to the current playback location.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
static let seek: GroupSessionEvent.Action
```

## See Also

### Getting playback-related actions

static let play: GroupSessionEvent.Action

An action that indicates the start of playback.

static let pause: GroupSessionEvent.Action

An action that indicates an end to playback.

static func skip(item: String) -> GroupSessionEvent.Action

Returns an event that indicates a skipped track or playback item.

