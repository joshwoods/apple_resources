

- MusicKit
- MusicPlayer
- MusicPlayer.Queue
- MusicPlayer.Queue.Entry
-  init(\_:startTime:endTime:) 

Initializer

# init(\_:startTime:endTime:)

Creates an entry of the playback queue with a playable music item, and optional start and end times.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 14.0+tvOS 15.0+visionOS 1.0+

``` source
init(
    _ playableMusicItem: any PlayableMusicItem,
    startTime: TimeInterval? = nil,
    endTime: TimeInterval? = nil
)
```

