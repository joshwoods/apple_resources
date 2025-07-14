

- Group Activities
- GroupSessionEvent
- GroupSessionEvent.Action
- GroupSessionEvent.Action.QueueChange
-  added(\_:) 

Type Method

# added(\_:)

Returns a queue change for an added item.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
static func added(_ item: GroupSessionEvent.Action.QueueChange.Item) -> GroupSessionEvent.Action.QueueChange
```

## Parameters 

`item`  

The item the participant added to the queue.

## Return Value

A type that contains information about the change.

## Discussion

Before showing a notice to the user, call this method to generate a type for the added item. Pass this type to the updatedQueue(_:) method to create the postable action.

## See Also

### Specifying the type of change

static func setUpNext(GroupSessionEvent.Action.QueueChange.Item) -> GroupSessionEvent.Action.QueueChange

Returns a queue change for a new up-next item.

