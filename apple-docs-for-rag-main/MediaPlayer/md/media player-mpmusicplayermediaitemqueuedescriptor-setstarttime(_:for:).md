

- Media Player
- MPMusicPlayerMediaItemQueueDescriptor
-  setStartTime(\_:for:) 

Instance Method

# setStartTime(\_:for:)

The time the designated media item is to start playing.

iOS 10.1+iPadOS 10.1+Mac Catalyst 13.1+visionOS 1.0+

``` source
func setStartTime(
    _ startTime: TimeInterval,
    for mediaItem: MPMediaItem
)
```

## Parameters 

`startTime`  

The TimeInterval describing when the media item starts playing.

`mediaItem`  

The media item in the queue that has a changed start time.

## See Also

### Setting start and end times

func setEndTime(TimeInterval, for: MPMediaItem)

The time the designated media item is to stop playing.

