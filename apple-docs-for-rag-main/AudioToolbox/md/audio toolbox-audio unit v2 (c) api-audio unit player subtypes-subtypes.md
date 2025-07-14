

- Audio Toolbox
- Audio Unit v2 (C) API
-  Audio Unit Player Subtypes 

API Collection

# Audio Unit Player Subtypes

## Topics

### Constants

var kAudioUnitSubType_AudioFilePlayer: UInt32

var kAudioUnitSubType_AudioFilePlayer: UInt32

var kAudioUnitSubType_NetReceive: UInt32

var kAudioUnitSubType_ScheduledSoundPlayer: UInt32

A generator unit that can be used to schedule slices of audio to be played at specified times. The audio is scheduled using the time stamps for the render operation and can be scheduled from any thread.

var kAudioUnitSubType_ScheduledSoundPlayer: UInt32

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

Audio Unit Pitch Subtypes

enum AudioUnitEventType

