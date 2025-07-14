

- Audio Toolbox
-  AURecordedParameterEvent 

Structure

# AURecordedParameterEvent

An event recording the changing of a parameter at a particular host time.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct AURecordedParameterEvent
```

## Topics

### Initializers

init()

init(hostTime: UInt64, address: AUParameterAddress, value: AUValue)

### Instance Properties

var address: AUParameterAddress

The address of the parameter whose value changed.

var hostTime: UInt64

The host time at which the event occurred.

var value: AUValue

The value of the parameter at the given time.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

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

