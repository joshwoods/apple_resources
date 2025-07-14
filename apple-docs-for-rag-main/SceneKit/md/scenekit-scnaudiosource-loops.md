

- SceneKit
- SCNAudioSource
-  loops 

Instance Property

# loops

A Boolean value that determines whether the audio source should play repeatedly.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var loops: Bool { get set }
```

## Discussion

If this value is true, audio players using this source automatically begin playing again after playback has finished. If this value is false (the default), the audio source plays exactly once.

## See Also

### Setting Default Playback Parameters

var volume: Float

The default playback volume for the audio source.

var rate: Float

The default playback rate for the audio source.

var reverbBlend: Float

The default blend of blend of unmodified and reverb-processed (also called dry and wet) audio for playback of the audio source.

var shouldStream: Bool

A Boolean value that determines whether the audio source should stream content from its source URL when playing.

