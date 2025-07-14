

- Media Player
- MPMusicPlayerControllerMutableQueue
-  insert(\_:after:) 

Instance Method

# insert(\_:after:)

Inserts a modified queue after the designated media item.

iOS 10.3+iPadOS 10.3+Mac Catalyst 13.1+tvOS 14.0+visionOS 1.0+

``` source
func insert(
    _ queueDescriptor: MPMusicPlayerQueueDescriptor,
    after afterItem: MPMediaItem?
)
```

## Parameters 

`queueDescriptor`  

A queue descriptor the system uses to insert media items in the playback queue.

`afterItem`  

The media item before the insertion point for the modified queue.

## See Also

### Adding and removing items

func remove(MPMediaItem)

Removes a media item from the music player’s queue.

