

- Audio Toolbox
-  AudioUnitParameterHistoryInfo 

Structure

# AudioUnitParameterHistoryInfo

The suggested update rate and history duration for parameters which have the flag_PlotHistory flag set.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct AudioUnitParameterHistoryInfo
```

## Overview

The structure is filled out by getting the value of the `kAudioUnitProperty_ParameterHistoryInfo` property.

## Topics

### Initializers

init()

init(updatesPerSecond: Float32, historyDurationInSeconds: Float32)

### Instance Properties

var historyDurationInSeconds: Float32

var updatesPerSecond: Float32

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

