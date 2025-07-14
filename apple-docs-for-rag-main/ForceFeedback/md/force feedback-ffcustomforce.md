

- Force Feedback
-  FFCUSTOMFORCE 

Structure

# FFCUSTOMFORCE

Contains type-specific information for the CUSTOMFORCE effect.

Mac Catalyst 13.0+macOS 10.2+

``` source
struct FFCUSTOMFORCE
```

## Overview

A pointer to a single FFCUSTOMFORCE structure for an effect is passed in the **lpvTypeSpecificParams** member of the FFEFFECT structure.

The structure describes a custom or user-defined force.

## Topics

### Initializers

init()

init(cChannels: DWORD, dwSamplePeriod: DWORD, cSamples: DWORD, rglForceData: LPLONG!)

### Instance Properties

var cChannels: DWORD

Number of channels (axes) affected by this force.

var cSamples: DWORD

Total number of samples in the **rglForceData**. It must be an integral multiple of the **cChannels**.

var dwSamplePeriod: DWORD

Sample period, in microseconds.

var rglForceData: LPLONG!

Pointer to an array of force values representing the custom force. If multiple channels are provided, the values are interleaved. For example, if **cChannels** is 3, the first element of the array belongs to the first channel, the second to the second, and the third to the third.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Data Types

struct FFCAPABILITIES

Used by the FFDeviceGetForceFeedbackCapabilities method to retrieve device force-feedback capabilities.

struct FFCONDITION

A structure containing type-specific information for certain effects.

struct FFCONSTANTFORCE

Contains type-specific information for the CONSTANTFORCE effect.

struct FFEFFECT

UsUsed by the FFDeviceCreateEffect method to initialize a new effect object. It is also used by the FFEffectSetParameters and FFEffectGetParameters functions.

struct FFEFFESCAPE

The FFEFFESCAPE structure passes hardware-specific data directly to the Force Feedback plugIn.

struct FFENVELOPE

Used by the FFEFFECT structure to specify the optional envelope parameters for an effect.

struct FFPERIODIC

A structure containing type-specific information for certain effects.

struct FFRAMPFORCE

Contains type-specific information for the RAMPFORCE effect.

