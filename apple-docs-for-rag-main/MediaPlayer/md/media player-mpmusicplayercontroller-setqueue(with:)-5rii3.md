

- Media Player
- MPMusicPlayerController
-  setQueue(with:) 

Instance Method

# setQueue(with:)

Sets a music player’s playback queue based on a media query.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func setQueue(with query: MPMediaQuery)
```

## Parameters 

`query`  

A media query that specifies the collection of media items that you want as the playback queue. See MPMediaQuery for a description of query types and how to create them.

## Discussion

To begin playback after establishing a playback queue, call prepareToPlay().

## See Also

### Setting up a playback queue

func setQueue(with: MPMediaItemCollection)

Sets a music player’s playback queue using a media item collection.

func setQueue(with: [String])

Sets a music player’s playback queue using with media items identified by the store identifiers.

func setQueue(with: MPMusicPlayerQueueDescriptor)

Set the music player’s playback queue using media items that fit the queue descriptor properties.

