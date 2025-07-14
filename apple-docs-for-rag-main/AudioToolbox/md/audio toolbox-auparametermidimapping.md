

- Audio Toolbox
-  AUParameterMIDIMapping 

Structure

# AUParameterMIDIMapping

macOS

``` source
struct AUParameterMIDIMapping
```

## Topics

### Initializers

init()

init(mScope: AudioUnitScope, mElement: AudioUnitElement, mParameterID: AudioUnitParameterID, mFlags: AUParameterMIDIMappingFlags, mSubRangeMin: AudioUnitParameterValue, mSubRangeMax: AudioUnitParameterValue, mStatus: UInt8, mData1: UInt8, reserved1: UInt8, reserved2: UInt8, reserved3: UInt32)

### Instance Properties

var mData1: UInt8

var mElement: AudioUnitElement

var mFlags: AUParameterMIDIMappingFlags

var mParameterID: AudioUnitParameterID

var mScope: AudioUnitScope

var mStatus: UInt8

var mSubRangeMax: AudioUnitParameterValue

var mSubRangeMin: AudioUnitParameterValue

var reserved1: UInt8

var reserved2: UInt8

var reserved3: UInt32

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

