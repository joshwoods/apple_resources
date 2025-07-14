

- SceneKit
- SCNAudioSource
-  rate 

Instance Property

# rate

The default playback rate for the audio source.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var rate: Float { get set }
```

## Discussion

This property determines the default rate for when a source begins playing. To vary the rate during playback through an SCNAudioPlayer object, use the player’s audioNode property to access real-time audio controls.

## See Also

### Setting Default Playback Parameters

var volume: Float

The default playback volume for the audio source.

var reverbBlend: Float

The default blend of blend of unmodified and reverb-processed (also called dry and wet) audio for playback of the audio source.

var loops: Bool

A Boolean value that determines whether the audio source should play repeatedly.

var shouldStream: Bool

A Boolean value that determines whether the audio source should stream content from its source URL when playing.

