

- Audio Toolbox
-  Audio Unit Properties 

API Collection

# Audio Unit Properties

Obtain information about the built-in mixers, equalizers, filters, effects, and other Audio Unit app extensions.

## Topics

### General

Other Plug-In Formats

RenderQuality

Render quality settings for audio units.

General Audio Unit Properties

Properties that apply to any audio unit.

struct HostCallbackInfo

The time- and transport-related callback functions for an audio unit.

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

Mixer Audio Unit Subtypes

Audio mixing audio unit subtypes for audio units provided by Apple.

enum AUSpatialMixerOutputType

enum AUSpatialMixerPointSourceInHeadMode

enum AUSpatialMixerSourceMode

3D Mixer Unit Parameters

Parameters for the 3D Mixer unit.

enum AU3DMixerAttenuationCurve

struct AU3DMixerRenderingFlags

struct MixerDistanceParams

### Equalizers

Parametric EQ Unit Parameters

Parameters for the Parametric EQ unit.

Audio Unit Graphic EQ Parameter ID

Peak Limiter Unit Parameters

Parameters for the Peak Limiter unit.

Dynamics Processor Unit Parameters

Parameters for the Dynamics Processor unit.

Frequency Response Constants

The maximum number of frequency response bin structures for the `AudioUnitProperty_FrequencyResponse` property.

enum AUSpatializationAlgorithm

### Filters

Audio Unit Filter Subtypes

Bandpass Unit Parameters

Parameters for the Bandpass unit.

AUHipass Parameters

Parameters for the Highpass unit.

AULowpass Parameters

Parameters for the Lowpass unit.

AULowShelf Parameters

Parameters for the Low Shelf Filter unit.

AUHighShelfFilter Parameters

Parameters for the High Shelf Filter unit.

AUNBandEQ Filter Types

Values for the filter type parameter of the Multitype EQ (NBandEQ) unit.

AUNBandEQ Property IDs

AUNBandEQ Parameters

### Effects

Effect Audio Unit Subtypes

Effect (digital signal processing) audio unit subtypes for audio units provided by Apple.

AUMatrixReverb Parameters

AUDistortion Parameters

Reverb Parameters

Additional reverb parameters.

Reverb Unit Parameters

Parameters for the Reverb unit.

enum AUReverbRoomType

Varispeed Unit Parameters

Parameters for the Varispeed unit.

AUDelay Parameters

AUMultibandCompressor Parameters

AUDeferredRenderer Properties

AUSampleDelay Parameters

AUNewTimePitch Parameters

AUTimePitch, AUTimePitch (offline), and AUPitch Unit Parameters

### Input/Output

I/O Audio Unit Properties

Properties for Apple I/O audio units (sometimes called output units).

Inter-App Output Unit Property IDs

Inter-App Audio Unit Property IDs

Output Unit Parameters

AUNetReceive Properties

AUNetSend Properties

AUNetSend Parameters

AUNetReceive Parameters

AUNetSendPresetFormat Properties

Net Status Audio Unit Parameters

I/O Audio Unit Function Selectors

Audio unit component selectors, specific to I/O audio units, that correspond to functions in the audio unit API.

struct AudioOutputUnitMIDICallbacks

struct AudioOutputUnitStartAtTimeParams

A timestamp for scheduled starting of an I/O audio unit.

### Generators

AURandom Parameters

AUSampler Parameters

AUSampler Property IDs

AUSampler Properties

AURogerBeep Parameters

AUMIDISynth Properties

AURoundTripAACParam Parameters

## See Also

### Audio Units

Generating spatial audio from a multichannel audio stream

Convert 8-channel audio to 2-channel spatial audio by using a spatial mixer audio unit.

Audio Unit v3 Plug-Ins

Deliver custom audio effects, instruments, and other audio behaviors using an Audio Unit v3 app extension.

Audio Components

Find, load, and configure audio components, such as Audio Units and audio codecs.

Audio Unit v2 (C) API

Configure an Audio Unit and prepare it to render audio.

Audio Unit Voice I/O

Configure system voice processing and respond to speech events.

