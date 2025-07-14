

- Group Activities
- GroupSessionEvent
- GroupSessionEvent.Action
-  updatedQueue 

Type Property

# updatedQueue

An action that represents a nonspecific change to the queue.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
static let updatedQueue: GroupSessionEvent.Action
```

## Discussion

Use this action when the other action types don’t accurately describe the change you made to the queue. If you can specify the change using a GroupSessionEvent.Action.QueueChange type, use the updatedQueue(_:) method instead.

## See Also

### Getting change-related actions

static func updatedQueue(GroupSessionEvent.Action.QueueChange) -> GroupSessionEvent.Action

Returns an action that represents a change to the playback queue.

struct QueueChange

A type that describes a modification to the playback queue.

