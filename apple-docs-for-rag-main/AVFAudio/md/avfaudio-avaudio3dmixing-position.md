

- AVFAudio
- AVAudio3DMixing
-  position 

Instance Property

# position

The location of the source in the 3D environment.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var position: AVAudio3DPoint { get set }
```

**Required**

## Discussion

The system specifies the coordinates in meters. Only the AVAudioEnvironmentNode class implements this property.

## See Also

### Getting the 3D Mixing Parameters

var obstruction: Float

A value that simulates filtering of the direct path of sound due to an obstacle.

**Required**

var occlusion: Float

A value that simulates filtering of the direct and reverb paths of sound due to an obstacle.

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

