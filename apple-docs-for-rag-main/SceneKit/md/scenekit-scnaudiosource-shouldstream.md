

- SceneKit
- SCNAudioSource
-  shouldStream 

Instance Property

# shouldStream

A Boolean value that determines whether the audio source should stream content from its source URL when playing.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var shouldStream: Bool { get set }
```

## Discussion

If this value is true, audio players using this source do not preload audio buffer data, instead reading directly from the source file while playing audio. If this value is false, SceneKit loads audio buffer data upon playing audio from the source.

## See Also

### Setting Default Playback Parameters

var volume: Float

The default playback volume for the audio source.

var rate: Float

The default playback rate for the audio source.

var reverbBlend: Float

The default blend of blend of unmodified and reverb-processed (also called dry and wet) audio for playback of the audio source.

var loops: Bool

A Boolean value that determines whether the audio source should play repeatedly.

