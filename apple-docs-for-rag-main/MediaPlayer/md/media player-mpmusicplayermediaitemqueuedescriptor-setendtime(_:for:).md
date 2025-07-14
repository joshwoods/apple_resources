

- Media Player
- MPMusicPlayerMediaItemQueueDescriptor
-  setEndTime(\_:for:) 

Instance Method

# setEndTime(\_:for:)

The time the designated media item is to stop playing.

iOS 10.1+iPadOS 10.1+Mac Catalyst 13.1+visionOS 1.0+

``` source
func setEndTime(
    _ endTime: TimeInterval,
    for mediaItem: MPMediaItem
)
```

## Parameters 

`endTime`  

The TimeInterval describing when the media item stops playing.

`mediaItem`  

The media item in the queue that has a changed end time.

## See Also

### Setting start and end times

func setStartTime(TimeInterval, for: MPMediaItem)

The time the designated media item is to start playing.

