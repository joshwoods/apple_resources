

- Audio Toolbox
-  AUHostTransportStateFlags 

Structure

# AUHostTransportStateFlags

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct AUHostTransportStateFlags
```

## Topics

### Constants

static var changed: AUHostTransportStateFlags

Indicates such state changes as start, stop, or seeking to another position in the timeline. Can be active if there was a change to the state of, or discontinuities in, the audio transport since the AUHostTransportStateBlock callback was last called.

static var cycling: AUHostTransportStateFlags

Indicates that the host is cycling or looping.

static var moving: AUHostTransportStateFlags

Indicates that the audio transport is moving.

static var recording: AUHostTransportStateFlags

Indicates that the host is recording, or is prepared to record. Can be active with or without a moving state.

### Initializers

init(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Structures

struct AudioUnitConnection

An audio unit source-to-destination connection specification.

struct AudioUnitEvent

struct AudioUnitExternalBuffer

Allows an audio unit host application to tell an audio unit to use a specified buffer for its input callback.

struct AudioUnitFrequencyResponseBin

An audio unit’s audio level at a particular frequency.

struct AudioUnitMeterClipping

Audio clipping that has occurred in a mixer unit.

struct AudioUnitMIDIControlMapping

struct AudioUnitOtherPluginDesc

struct AudioUnitParameter

An adjustable audio unit attribute such as volume, pitch, or filter cutoff frequency.

struct AudioUnitParameterEvent

A scheduled change to an audio unit parameter’s value.

struct AudioUnitParameterHistoryInfo

The suggested update rate and history duration for parameters which have the flag_PlotHistory flag set.

struct AudioUnitParameterNameInfo

A short version of the name for an audio unit parameter.

typealias AudioUnitParameterIDName

A type definition for a data type that defines the short version of the name for an audio unit parameter.

struct AudioUnitParameterInfo

struct AudioUnitParameterOptions

Value options for audio unit parameters.

struct AudioUnitParameterStringFromValue

A string representation of a parameter’s value.

