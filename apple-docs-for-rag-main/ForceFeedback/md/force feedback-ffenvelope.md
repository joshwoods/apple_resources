

- Force Feedback
-  FFENVELOPE 

Structure

# FFENVELOPE

Used by the FFEFFECT structure to specify the optional envelope parameters for an effect.

Mac Catalyst 13.0+macOS 10.2+

``` source
struct FFENVELOPE
```

## Overview

The sustain level for the envelope is represented by the **dwMagnitude** member of the FFPERIODIC structure and the **lMagnitude** member of the FFCONSTANTFORCE structure. The sustain time is represented by **dwDuration** member of the FFEFFECT structure

## Topics

### Initializers

init()

init(dwSize: DWORD, dwAttackLevel: DWORD, dwAttackTime: DWORD, dwFadeLevel: DWORD, dwFadeTime: DWORD)

### Instance Properties

var dwAttackLevel: DWORD

Amplitude for the start of the envelope, relative to the baseline, in the range from 0 through 10,000. If the effect’s type-specific data does not specify a baseline, the amplitude is relative to 0.

var dwAttackTime: DWORD

The time, in microseconds, to reach the sustain level.

var dwFadeLevel: DWORD

Amplitude for the end of the envelope, relative to the baseline, in the range from 0 through 10,000. If the effect’s type-specific data does not specify a baseline, the amplitude is relative to 0.

var dwFadeTime: DWORD

The time, in microseconds, to reach the fade level.

var dwSize: DWORD

Size, in bytes, of this structure. This member must be initialized before the structure is used.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Data Types

struct FFCAPABILITIES

Used by the FFDeviceGetForceFeedbackCapabilities method to retrieve device force-feedback capabilities.

struct FFCONDITION

A structure containing type-specific information for certain effects.

struct FFCONSTANTFORCE

Contains type-specific information for the CONSTANTFORCE effect.

struct FFCUSTOMFORCE

Contains type-specific information for the CUSTOMFORCE effect.

struct FFEFFECT

UsUsed by the FFDeviceCreateEffect method to initialize a new effect object. It is also used by the FFEffectSetParameters and FFEffectGetParameters functions.

struct FFEFFESCAPE

The FFEFFESCAPE structure passes hardware-specific data directly to the Force Feedback plugIn.

struct FFPERIODIC

A structure containing type-specific information for certain effects.

struct FFRAMPFORCE

Contains type-specific information for the RAMPFORCE effect.

