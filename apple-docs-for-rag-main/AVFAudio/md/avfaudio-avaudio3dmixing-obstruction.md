

- AVFAudio
- AVAudio3DMixing
-  obstruction 

Instance Property

# obstruction

A value that simulates filtering of the direct path of sound due to an obstacle.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var obstruction: Float { get set }
```

**Required**

## Discussion

The value of `obstruction` is in decibels. The system blocks only the direct path of sound between the source and listener.

The default value is `0.0`, and the range of valid values is `-100` to `0`. Only the AVAudioEnvironmentNode class implements this property.

## See Also

### Getting the 3D Mixing Parameters

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

var reverbBlend: Float

A value that controls the blend of dry and reverb processed audio.

**Required**

var sourceMode: AVAudio3DMixingSourceMode

The source mode for the input bus of the audio environment node.

**Required**

