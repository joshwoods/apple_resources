

- RealityKit
- AudioPlaybackController
-  pause() 

Instance Method

# pause()

Pauses playback of the audio resource while maintaining the position in the audio stream.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func pause()
```

## Discussion

Resume playback of a paused audio resource by calling the play() method.

## See Also

### Starting and stopping audio playback

func play()

Plays the audio resource.

func stop()

Stops playback of the audio resource and discards the location in the audio stream.

var isPlaying: Bool

A Boolean value that indicates whether playback is currently active.

