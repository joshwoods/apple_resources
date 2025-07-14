

- Audio Toolbox
-  AudioUnitParameter 

Structure

# AudioUnitParameter

An adjustable audio unit attribute such as volume, pitch, or filter cutoff frequency.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct AudioUnitParameter
```

## Overview

This data structure is used by functions declared in the `AudioToolbox/AudioUnitUtilities.h` header file in macOS.

An audio unit parameter is uniquely identified by the combination of its scope, element, and ID.

## Topics

### Initializers

init(mAudioUnit: AudioUnit, mParameterID: AudioUnitParameterID, mScope: AudioUnitScope, mElement: AudioUnitElement)

init(mAudioUnit: AudioUnit, mParameterID: AudioUnitParameterID, mScope: AudioUnitScope, mElement: AudioUnitElement)

### Instance Properties

var mAudioUnit: AudioUnit

The audio unit instance that the parameter applies to.

var mElement: AudioUnitElement

The audio unit element for the parameter.

var mParameterID: AudioUnitParameterID

The audio unit parameter identifier.

var mScope: AudioUnitScope

The audio unit scope for the parameter.

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

struct AudioUnitParameterValueFromString

A parameter’s value based on a string representation of the value.

