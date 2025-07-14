

- Audio Toolbox
- Audio Unit v2 (C) API
-  General Audio Unit Function Selectors 

API Collection

# General Audio Unit Function Selectors

General audio unit component selectors that correspond to functions in the audio unit API.

## Topics

### Constants

var kAudioUnitAddPropertyListenerSelect: Int

Used by the system to register a property listener callback function for an audio unit when you call the AudioUnitAddPropertyListener(_:_:_:_:) function.

var kAudioUnitAddRenderNotifySelect: Int

var kAudioUnitComplexRenderSelect: Int

var kAudioUnitGetParameterSelect: Int

Used by the system to get the current value of an audio unit parameter when you call the AudioUnitGetParameter(_:_:_:_:_:) function.

var kAudioUnitGetPropertyInfoSelect: Int

Used by the system to get property information from an audio unit when you call the AudioUnitGetPropertyInfo(_:_:_:_:_:_:) function.

var kAudioUnitGetPropertySelect: Int

var kAudioUnitInitializeSelect: Int

var kAudioUnitProcessMultipleSelect: Int

var kAudioUnitProcessSelect: Int

var kAudioUnitRange: Int

var kAudioUnitRemovePropertyListenerSelect: Int

Used by the system to unregister a property listener callback function from an audio unit when you call the `AudioUnitRemovePropertyListener` function.

var kAudioUnitRemovePropertyListenerWithUserDataSelect: Int

var kAudioUnitRemoveRenderNotifySelect: Int

var kAudioUnitRenderSelect: Int

Used by the system to invoke audio rendering by an audio unit when you call the AudioUnitRender(_:_:_:_:_:_:) function.

var kAudioUnitResetSelect: Int

Used by the system to reset an audio unit when you call the AudioUnitReset(_:_:_:) function.

var kAudioUnitScheduleParametersSelect: Int

Used by the system to schedule an audio unit parameter value change when you call the AudioUnitScheduleParameters(_:_:_:) function.

var kAudioUnitSetParameterSelect: Int

Used by the system to set the value of an audio unit parameter when you call the AudioUnitSetParameter(_:_:_:_:_:_:) function.

var kAudioUnitSetPropertySelect: Int

var kAudioUnitUninitializeSelect: Int

Used by the system to uninitialize an audio unit when you call the AudioUnitUninitialize(_:) function.

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

Generator Audio Unit Subtypes

Audio units that serve as sound sources.

Input/Output Audio Unit Subtypes

Input/output audio unit subtypes for audio units provided by Apple.

Audio Unit Panner Subtypes

Audio Unit Player Subtypes

Audio Unit Pitch Subtypes

enum AudioUnitEventType

