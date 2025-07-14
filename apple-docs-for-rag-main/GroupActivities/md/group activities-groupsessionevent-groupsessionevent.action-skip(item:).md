

- Group Activities
- GroupSessionEvent
- GroupSessionEvent.Action
-  skip(item:) 

Type Method

# skip(item:)

Returns an event that indicates a skipped track or playback item.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
static func skip(item: String) -> GroupSessionEvent.Action
```

## Parameters 

`item`  

The name of the skipped item.

## Discussion

This function creates an action that represents a skipped playback item. If your app’s activity manages a playlist of items, you might use this action to indicate a participant skipped an item. For example, you might name a skipped song in a shared playlist.

## See Also

### Getting playback-related actions

static let play: GroupSessionEvent.Action

An action that indicates the start of playback.

static let pause: GroupSessionEvent.Action

An action that indicates an end to playback.

static let seek: GroupSessionEvent.Action

An event that indicates a change to the current playback location.

