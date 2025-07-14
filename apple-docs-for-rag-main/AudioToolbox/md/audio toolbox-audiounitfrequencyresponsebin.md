

- Audio Toolbox
-  AudioUnitFrequencyResponseBin 

Structure

# AudioUnitFrequencyResponseBin

An audio unit’s audio level at a particular frequency.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct AudioUnitFrequencyResponseBin
```

## Overview

An array of AudioUnitFrequencyResponseBin are passed in to kAudioUnitProperty_FrequencyResponse with the mFrequency field filled in. The array is returned with the mMagnitude fields filled in. If fewer than kNumberOfResponseFrequencies are needed, then the first unused bin should be marked with a negative frequency.

## Topics

### Initializers

init()

init(mFrequency: Float64, mMagnitude: Float64)

### Instance Properties

var mFrequency: Float64

var mMagnitude: Float64

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

struct AudioUnitParameterValueFromString

A parameter’s value based on a string representation of the value.

