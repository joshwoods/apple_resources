

- Group Activities
- GroupSessionEvent
- 
  - GroupSessionEvent
- GroupSessionEvent.Action
- GroupSessionEvent.Action.QueueChange
- GroupSessionEvent.Action.QueueChange.Item
-  container(\_:) 

Type Method

# container(\_:)

Creates an item that contains the name of a container.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
static func container(_ name: String) -> GroupSessionEvent.Action.QueueChange.Item
```

## Parameters 

`name`  

The name of the container.

## Discussion

When a participant changes an entire queue, call this method to create an item with the queue name. When you show the change notice, SharePlay displays the container name to the participant.

## See Also

### Creating the item

static func song(String) -> GroupSessionEvent.Action.QueueChange.Item

Creates an item that contains the name of a song.

