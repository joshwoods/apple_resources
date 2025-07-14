

- Force Feedback
-  FFCONSTANTFORCE 

Structure

# FFCONSTANTFORCE

Contains type-specific information for the CONSTANTFORCE effect.

Mac Catalyst 13.0+macOS 10.2+

``` source
struct FFCONSTANTFORCE
```

## Overview

A pointer to a single FFCONSTANTFORCE structure for an effect is passed in the **lpvTypeSpecificParams** member of the FFEFFECT structure.

## Topics

### Initializers

init()

init(lMagnitude: LONG)

### Instance Properties

var lMagnitude: LONG

The magnitude of the effect, in the range from -10,000 through 10,000. If an envelope is applied to this effect, the value represents the magnitude of the sustain. If no envelope is applied, the value represents the amplitude of the entire effect.

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

struct FFCUSTOMFORCE

Contains type-specific information for the CUSTOMFORCE effect.

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

