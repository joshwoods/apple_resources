

- MusicKit
- MusicPlayer
-  skipToPreviousEntry() 

Instance Method

# skipToPreviousEntry()

Starts playback of the previous entry in the playback queue.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 14.0+tvOS 15.0+visionOS 1.0+

``` source
func skipToPreviousEntry() async throws
```

## Discussion

If the music player isn’t playing, this method designates the previous entry as the next to play.

When you call this method, playback ends if the music player is already at the first entry in the playback queue.

