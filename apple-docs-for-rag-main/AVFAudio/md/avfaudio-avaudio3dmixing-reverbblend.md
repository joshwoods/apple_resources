

- AVFAudio
- AVAudio3DMixing
-  reverbBlend 

Instance Property

# reverbBlend

A value that controls the blend of dry and reverb processed audio.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var reverbBlend: Float { get set }
```

**Required**

## Discussion

This property controls the amount of the source’s audio that the AVAudioEnvironmentNode instance processes. A value of `0.5` results in an equal blend of dry and processed (wet) audio.

The default is `0.0`, and the range of valid values is `0.0` (completely dry) to `1.0` (completely wet). Only the AVAudioEnvironmentNode class implements this property.

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

var pointSourceInHeadMode: AVAudio3DMixingPointSourceInHeadMode

The in-head mode for a point source.

**Required**

var sourceMode: AVAudio3DMixingSourceMode

The source mode for the input bus of the audio environment node.

**Required**

