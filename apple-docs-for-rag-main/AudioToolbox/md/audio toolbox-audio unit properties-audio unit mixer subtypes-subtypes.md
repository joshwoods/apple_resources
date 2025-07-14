

- Audio Toolbox
- Audio Unit Properties
-  Audio Unit Mixer Subtypes 

API Collection

# Audio Unit Mixer Subtypes

## Topics

### Constants

var kAudioUnitSubType_3DMixer: UInt32

An audio unit that can have any number of input buses and one output bus. Each input bus can be mono, in which case it can be panned using 3D coordinates and parameters. Stereo input buses pass directly through to the output. Four-channel *ambisonic* inputs are rendered to the output configuration. The single output bus can be configured with 2, 4, 5, 6, 7 or 8 channels.

Deprecated

var kAudioUnitSubType_StereoMixer: UInt32

An audio unit that can have any number of input buses, each of which is mono or stereo, and one stereo output bus.

## See Also

### Mixers

enum AUSpatialMixerAttenuationCurve

struct AUSpatialMixerRenderingFlags

AUSpatialMixer Parameters

Panner Audio Unit Parameters

AUMatrixMixer Parameters

AUMultiChannelMixer Parameters

Parameters for the Multichannel Mixer unit.

Spatial Mixer Property IDs

Stereo Mixer Unit Parameters

Mixer Audio Unit Properties

Properties for Apple mixer audio units.

Mixer Audio Unit Subtypes

Audio mixing audio unit subtypes for audio units provided by Apple.

enum AUSpatialMixerOutputType

enum AUSpatialMixerPointSourceInHeadMode

enum AUSpatialMixerSourceMode

3D Mixer Unit Parameters

Parameters for the 3D Mixer unit.

enum AU3DMixerAttenuationCurve

