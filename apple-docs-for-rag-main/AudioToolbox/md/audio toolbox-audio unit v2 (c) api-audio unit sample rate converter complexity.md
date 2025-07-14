

- Audio Toolbox
- Audio Unit v2 (C) API
-  Audio Unit Sample Rate Converter Complexity 

API Collection

# Audio Unit Sample Rate Converter Complexity

Quality levels for the audio sample-rate conversion algorithm.

## Topics

### Constants

var kAudioUnitSampleRateConverterComplexity_Linear: UInt32

Basic sample rate conversion using linear interpolation. Fast, but lower quality.

var kAudioUnitSampleRateConverterComplexity_Mastering: UInt32

Mastering quality sample rate conversion. More computationally expensive.

var kAudioUnitSampleRateConverterComplexity_Normal: UInt32

## See Also

### Enumerations

Audio Unit Types

The defined types of audio processing plug-ins known as audio units.

Inter-App Audio Unit Types

Audio Unit Manufacturer Identifier

The Apple audio unit manufacturer code.

Audio Unit Output Subtypes

I/O Audio Unit Subtypes

Converter Audio Unit Subtypes

Audio data format converter audio unit subtypes for audio units provided by Apple.

Reserved Audio Unit Clump Identifier

Reserved for system use.

Offline Audio Unit Properties

Properties for audio units that perform offline processing—that is, processing in a nonplayback, nonrealtime mode.

MIDI Audio Unit Parameters

Parameters for instrument units.

General Audio Unit Function Selectors

General audio unit component selectors that correspond to functions in the audio unit API.

Generator Audio Unit Subtypes

Audio units that serve as sound sources.

Input/Output Audio Unit Subtypes

Input/output audio unit subtypes for audio units provided by Apple.

Audio Unit Panner Subtypes

Audio Unit Player Subtypes

Audio Unit Pitch Subtypes

