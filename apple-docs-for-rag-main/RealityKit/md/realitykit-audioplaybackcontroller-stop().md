

- RealityKit
- AudioPlaybackController
-  stop() 

Instance Method

# stop()

Stops playback of the audio resource and discards the location in the audio stream.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func stop()
```

## Discussion

The next time you call play(), playback starts at the beginning of the stream.

## See Also

### Starting and stopping audio playback

func play()

Plays the audio resource.

func pause()

Pauses playback of the audio resource while maintaining the position in the audio stream.

var isPlaying: Bool

A Boolean value that indicates whether playback is currently active.

