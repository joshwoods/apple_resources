

- AVFAudio
- AVAudio3DMixing
-  pointSourceInHeadMode 

Instance Property

# pointSourceInHeadMode

The in-head mode for a point source.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var pointSourceInHeadMode: AVAudio3DMixingPointSourceInHeadMode { get set }
```

**Required**

## See Also

### Getting the 3D Mixing Parameters

var obstruction: Float

A value that simulates filtering of the direct path of sound due to an obstacle.

**Required**

var occlusion: Float

A value that simulates filtering of the direct and reverb paths of sound due to an obstacle.

**Required**

var position: AVAudio3DPoint

The location of the source in the 3D environment.

**Required**

var rate: Float

A value that changes the playback rate of the input signal.

**Required**

var reverbBlend: Float

A value that controls the blend of dry and reverb processed audio.

**Required**

var sourceMode: AVAudio3DMixingSourceMode

The source mode for the input bus of the audio environment node.

**Required**

