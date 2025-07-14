

- Audio Toolbox
-  AUParameterEventType 

Enumeration

# AUParameterEventType

Audio unit parameter event types.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
enum AUParameterEventType
```

## Topics

### Constants

case parameterEvent_Immediate

An immediate change from the parameter’s previous value to a new value.

case parameterEvent_Ramped

A gradual change from the parameter’s previous value to a new value, applied linearly over a specified period of time

### Initializers

init?(rawValue: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

