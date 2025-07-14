

- Media Player
- MPMusicPlayerController
-  setQueue(with:) 

Instance Method

# setQueue(with:)

Sets a music player’s playback queue using with media items identified by the store identifiers.

iOS 9.3+iPadOS 9.3+Mac Catalyst 13.1+tvOS 14.0+visionOS 1.0+

``` source
func setQueue(with storeIDs: [String])
```

## Parameters 

`storeIDs`  

An array of store identifiers associated with the media items to add to the queue.

## Discussion

To begin playback after establishing a playback queue, call prepareToPlay().

## See Also

### Setting up a playback queue

func setQueue(with: MPMediaQuery)

Sets a music player’s playback queue based on a media query.

func setQueue(with: MPMediaItemCollection)

Sets a music player’s playback queue using a media item collection.

func setQueue(with: MPMusicPlayerQueueDescriptor)

Set the music player’s playback queue using media items that fit the queue descriptor properties.

