

- AVFAudio
- AVAudio3DMixing
-  rate 

Instance Property

# rate

A value that changes the playback rate of the input signal.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var rate: Float { get set }
```

**Required**

## Discussion

A value of `2.0` results in the output audio playing one octave higher. A value of `0.5` results in the output audio playing one octave lower.

The default value is `1.0`, and the range of valid values is `0.5` to `2.0`. Only the AVAudioEnvironmentNode class implements this property.

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

var pointSourceInHeadMode: AVAudio3DMixingPointSourceInHeadMode

The in-head mode for a point source.

**Required**

var reverbBlend: Float

A value that controls the blend of dry and reverb processed audio.

**Required**

var sourceMode: AVAudio3DMixingSourceMode

The source mode for the input bus of the audio environment node.

**Required**

