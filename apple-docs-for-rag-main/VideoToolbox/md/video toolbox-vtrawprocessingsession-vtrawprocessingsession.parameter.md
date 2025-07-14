

- Video Toolbox
- VTRAWProcessingSession
-  VTRAWProcessingSession.Parameter 

Enumeration

# VTRAWProcessingSession.Parameter

A parameter expresses a control or a set of controls that influence frame processing.

macOS 15.0+

``` source
enum Parameter
```

## Overview

Parameters can represent Boolean options, integer or floating-point ranges, lists, or subgroups. All parameters have a collection of VTRAWProcessingSession.Parameter.Details containing a localized name suitable for display in UI, a longer localized description string, and a Boolean that indicates whether it’s enabled. All details, except for subgroups, must have a “key” string used to uniquely identify that parameter. All parameters other than subgroups have a collection of VTRAWProcessingSession.Parameter.Values containing a mandatory “initial” value, and optional “neutral” and “camera” values. VTRAWProcessingSession.Parameter.IntegerParameter and VTRAWProcessingSession.Parameter.FloatParameter are required to have “minimum” and “maximum” values in their Values

Parameter arrays are created and returned by the VideoToolbox framework.

## Topics

### Parameters

struct BooleanParameter

struct Details

struct FloatParameter

struct IntegerParameter

struct ListParameter

struct Values

### Enumeration Cases

case bool(VTRAWProcessingSession.Parameter.BooleanParameter)

case float(VTRAWProcessingSession.Parameter.FloatParameter)

case int(VTRAWProcessingSession.Parameter.IntegerParameter)

case list(VTRAWProcessingSession.Parameter.ListParameter)

case subgroup(details: VTRAWProcessingSession.Parameter.Details, elements: [VTRAWProcessingSession.Parameter])

## Relationships

### Conforms To

- Equatable
- Sendable

## See Also

### Configuring parameters

func parameters() -> any AsyncSequence&lt;[VTRAWProcessingSession.Parameter], Never>

Returns an asynchronous sequence that provides updates to the processing Parameter array if the processing extension makes changes to the set of Parameters.

func updateParameter(values: [String : Any]) throws

Sets the value for one or more of the processing parameters.

var processingParameters: [VTRAWProcessingSession.Parameter]

An array of processing parameters available for this RAW processing session.

