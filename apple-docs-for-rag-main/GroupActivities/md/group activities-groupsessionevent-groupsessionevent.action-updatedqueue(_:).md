

- Group Activities
- GroupSessionEvent
- GroupSessionEvent.Action
-  updatedQueue(\_:) 

Type Method

# updatedQueue(\_:)

Returns an action that represents a change to the playback queue.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
static func updatedQueue(_ change: GroupSessionEvent.Action.QueueChange) -> GroupSessionEvent.Action
```

## Parameters 

`change`  

The change that ocurred to the queue.

## Discussion

When you want to notify the user of changes to the playback queue, call this method to create an action type with the details of the change. Then call the showNotice(_:) method to post that action. For example, use the following code to notify the user that someone added a song to the queue.

```
groupSession.showNotice(.updatedQueue(.added(.song("Here comes the sun"))))
```

## See Also

### Getting change-related actions

static let updatedQueue: GroupSessionEvent.Action

An action that represents a nonspecific change to the queue.

struct QueueChange

A type that describes a modification to the playback queue.

