

- RealityKit
- AudioPlaybackController
-  isPlaying 

Instance Property

# isPlaying

A Boolean value that indicates whether playback is currently active.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
var isPlaying: Bool { get }
```

## Discussion

You may experience a small delay between when you call the play() method and when the isPlaying property reports `true`.

## See Also

### Starting and stopping audio playback

func play()

Plays the audio resource.

func pause()

Pauses playback of the audio resource while maintaining the position in the audio stream.

func stop()

Stops playback of the audio resource and discards the location in the audio stream.

