

- Audio Toolbox
- Audio Unit v2 (C) API
-  Audio Unit Scopes 

API Collection

# Audio Unit Scopes

Programmatic roles and contexts for audio unit properties.

## Topics

### Constants

var kAudioUnitScope_Global: AudioUnitScope

var kAudioUnitScope_Group: AudioUnitScope

In macOS, a context specific to the control scope of audio unit parameters.

var kAudioUnitScope_Input: AudioUnitScope

The context for audio data coming into an audio unit.

var kAudioUnitScope_Layer: AudioUnitScope

var kAudioUnitScope_LayerItem: AudioUnitScope

var kAudioUnitScope_Note: AudioUnitScope

In macOS, a scope for changes to an individual musical note. The element identifier used with this scope is the unique note identifier returned from a started note (see the `MusicDeviceStartNote` function in `AudioUnit/MusicDevice.h`).

var kAudioUnitScope_Output: AudioUnitScope

The context for audio data leaving an audio unit.

var kAudioUnitScope_Part: AudioUnitScope

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

