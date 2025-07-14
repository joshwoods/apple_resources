

- Media Player
- MPMusicPlayerController
-  setQueue(with:) 

Instance Method

# setQueue(with:)

Sets a music player’s playback queue using a media item collection.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func setQueue(with itemCollection: MPMediaItemCollection)
```

## Parameters 

`itemCollection`  

A media item collection that you want as the playback queue. See MPMediaItemCollection for a description of media item collections and how to use them.

## Discussion

To begin playback after establishing a playback queue, call prepareToPlay().

## See Also

### Setting up a playback queue

func setQueue(with: MPMediaQuery)

Sets a music player’s playback queue based on a media query.

func setQueue(with: [String])

Sets a music player’s playback queue using with media items identified by the store identifiers.

func setQueue(with: MPMusicPlayerQueueDescriptor)

Set the music player’s playback queue using media items that fit the queue descriptor properties.

