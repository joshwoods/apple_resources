

- Media Player
- MPMusicPlayerController
-  setQueue(with:) 

Instance Method

# setQueue(with:)

Set the music player’s playback queue using media items that fit the queue descriptor properties.

iOS 10.1+iPadOS 10.1+Mac Catalyst 13.1+tvOS 14.0+visionOS 1.0+

``` source
func setQueue(with descriptor: MPMusicPlayerQueueDescriptor)
```

## Parameters 

`descriptor`  

A queue descriptor the system uses to add media items to the playback queue.

## Discussion

To begin playback after establishing a playback queue, call prepareToPlay().

## See Also

### Setting up a playback queue

func setQueue(with: MPMediaQuery)

Sets a music player’s playback queue based on a media query.

func setQueue(with: MPMediaItemCollection)

Sets a music player’s playback queue using a media item collection.

func setQueue(with: [String])

Sets a music player’s playback queue using with media items identified by the store identifiers.

