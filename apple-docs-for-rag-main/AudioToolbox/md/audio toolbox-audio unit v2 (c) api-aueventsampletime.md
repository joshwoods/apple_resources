

- Audio Toolbox
- Audio Unit v2 (C) API
-  AUEventSampleTime 

API Collection

# AUEventSampleTime

Expresses time as a sample count.

## Overview

Callers of the AUScheduleParameterBlock and AUScheduleMIDIEventBlock blocks can pass the `AUEventSampleTimeImmediate` value to indicate that the event should be rendered as soon as possible (in the next cycle). A caller may also add a small (less than 4096) sample frame offset to this constant.

Note

The base AUAudioUnit implementation translates the `AUEventSampleTimeImmediate` constant to a true AUEventSampleTime value. Subclasses will not see this value.

## Topics

### Constants

var AUEventSampleTimeImmediate: AUEventSampleTime

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

