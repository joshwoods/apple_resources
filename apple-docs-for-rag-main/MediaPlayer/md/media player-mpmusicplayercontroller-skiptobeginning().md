

- Media Player
- MPMusicPlayerController
-  skipToBeginning() 

Instance Method

# skipToBeginning()

Restarts playback at the beginning of the currently playing media item.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOS 14.0+visionOS 1.0+

``` source
func skipToBeginning()
```

## See Also

### Controlling playback

func skipToNextItem()

Starts playback of the next media item in the playback queue, or if the music player isn’t playing, designates the next media item as the next item to play.

func skipToPreviousItem()

Starts playback of the previous media item in the playback queue, or if the music player isn’t playing, designates the previous media item as the next to play.

func append(MPMusicPlayerQueueDescriptor)

Inserts the media items defined by the queue descriptor after the last media item in the current queue.

func prepend(MPMusicPlayerQueueDescriptor)

Inserts the media items defined by the queue descriptor into the current queue immediately after the currently playing media item.

