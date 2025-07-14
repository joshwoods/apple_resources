

- MusicKit
- MusicPlayer
-  play() 

Instance Method

# play()

Initiates playback from the current queue.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 14.0+tvOS 15.0+visionOS 1.0+

``` source
func play() async throws
```

## Discussion

If playback isn’t underway, this method resumes playback from its paused location; otherwise, this method plays the first available entry from the beginning.

If a music player isn’t ready for playback when you call this method, this method prepares the music player and then starts playback.

