

- Audio Toolbox
-  AudioUnitParameterEvent 

Structure

# AudioUnitParameterEvent

A scheduled change to an audio unit parameter’s value.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct AudioUnitParameterEvent
```

## Overview

If the `eventType` field value is AUParameterEventType.parameterEvent_Immediate, use the `immediate` structure in the `eventValues` union. If the event type is AUParameterEventType.parameterEvent_Ramped, use the `ramp` structure in the `eventValues` union.

Apply one or more AudioUnitParameterEvent events to an audio unit using the AudioUnitScheduleParameters(_:_:_:) function.

## Topics

### Fields

var scope: AudioUnitScope

The scope for this parameter event.

var element: AudioUnitElement

The element for this parameter event.

var parameter: AudioUnitParameterID

An identifier for this parameter event.

var eventType: AUParameterEventType

The type for this parameter event.

var eventValues: AudioUnitParameterEvent.__Unnamed_union_eventValues

The values for this parameter event.

### Initializers

init()

init(scope: AudioUnitScope, element: AudioUnitElement, parameter: AudioUnitParameterID, eventType: AUParameterEventType, eventValues: AudioUnitParameterEvent.__Unnamed_union_eventValues)

## Relationships

### Conforms To

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

