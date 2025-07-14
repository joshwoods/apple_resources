

- Audio Toolbox
- Audio Unit Properties
-  Mixer Audio Unit Subtypes 

API Collection

# Mixer Audio Unit Subtypes

Audio mixing audio unit subtypes for audio units provided by Apple.

## Topics

### Constants

var kAudioUnitSubType_MatrixMixer: UInt32

var kAudioUnitSubType_MultiChannelMixer: UInt32

An audio unit that can have any number of input buses, with any number of channels on each input bus, and one output bus. In macOS, the output bus can have any number of channels. In iOS, the output bus always has two channels.

var kAudioUnitSubType_SpatialMixer: UInt32

## See Also

### Mixers

Audio Unit Mixer Subtypes

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

enum AUSpatialMixerOutputType

enum AUSpatialMixerPointSourceInHeadMode

enum AUSpatialMixerSourceMode

3D Mixer Unit Parameters

Parameters for the 3D Mixer unit.

enum AU3DMixerAttenuationCurve

