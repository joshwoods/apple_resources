

- RealityKit
- AudioPlaybackController
-  play() 

Instance Method

# play()

Plays the audio resource.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func play()
```

## Discussion

The controller plays from the beginning of the resource, or from the point at which it was paused if you previously called the pause() method during playback. The controller ignores calls to play() when audio is already playing.

## See Also

### Starting and stopping audio playback

func pause()

Pauses playback of the audio resource while maintaining the position in the audio stream.

func stop()

Stops playback of the audio resource and discards the location in the audio stream.

var isPlaying: Bool

A Boolean value that indicates whether playback is currently active.

