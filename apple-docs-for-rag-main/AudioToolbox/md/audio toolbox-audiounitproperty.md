

- Audio Toolbox
-  AudioUnitProperty 

Structure

# AudioUnitProperty

A key-value pair that declares an attribute or behavior for an audio unit.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct AudioUnitProperty
```

## Topics

### Initializers

init(mAudioUnit: AudioUnit, mPropertyID: AudioUnitPropertyID, mScope: AudioUnitScope, mElement: AudioUnitElement)

init(mAudioUnit: AudioUnit, mPropertyID: AudioUnitPropertyID, mScope: AudioUnitScope, mElement: AudioUnitElement)

### Instance Properties

var mAudioUnit: AudioUnit

The audio unit instance that the parameter applies to.

var mElement: AudioUnitElement

The audio unit element for the property.

var mPropertyID: AudioUnitPropertyID

The audio unit property identifier.

var mScope: AudioUnitScope

The audio unit scope for the property.

## Relationships

### Conforms To

- BitwiseCopyable

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

