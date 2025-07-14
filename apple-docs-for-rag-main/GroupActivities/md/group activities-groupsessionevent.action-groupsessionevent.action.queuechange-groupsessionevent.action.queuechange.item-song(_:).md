

- Group Activities
- GroupSessionEvent
- 
  - GroupSessionEvent
- GroupSessionEvent.Action
- GroupSessionEvent.Action.QueueChange
- GroupSessionEvent.Action.QueueChange.Item
-  song(\_:) 

Type Method

# song(\_:)

Creates an item that contains the name of a song.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
static func song(_ name: String) -> GroupSessionEvent.Action.QueueChange.Item
```

## Parameters 

`name`  

The name of the song.

## Discussion

When a participant adds a song or changes the next song in the queue, call this method to create an item with the song name. When you show the change notice, SharePlay displays the song name to the participant.

## See Also

### Creating the item

static func container(String) -> GroupSessionEvent.Action.QueueChange.Item

Creates an item that contains the name of a container.

