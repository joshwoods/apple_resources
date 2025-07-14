

- Force Feedback
-  FFCONDITION 

Structure

# FFCONDITION

A structure containing type-specific information for certain effects.

Mac Catalyst 13.0+macOS 10.2+

``` source
struct FFCONDITION
```

## Overview

Used with the SPRING, DAMPER, INERTIA, and FRICTION effects.A pointer to an array of FFCONDITION structures for an effect is passed in the **lpvTypeSpecificParams** member of the FFEFFECT structure. The number of elements in the array must be either one, or equal to the number of axes associated with the effect.

Different types of conditions interpret the parameters differently, but the basic idea is that force resulting from a condition is equal to *A(q - q0)* where *A* is a scaling coefficient, *q* is some metric, and *q0* is the neutral value for that metric.

The preceding simplified formula must be adjusted if a nonzero deadband is provided. If the metric is less than **lOffset - lDeadBand**, the resulting force is given by the following formula:

*force* = **lNegativeCoefficient** \* (*q* - (**lOffset - lDeadBand**))

Similarly, if the metric is greater than **lOffset + lDeadBand**, the resulting force is given by the following formula:

*force* = **lPositiveCoefficient** \* (*q* - (**lOffset + lDeadBand**))

A spring condition uses axis position as the metric.

A damper condition uses axis velocity as the metric.

An inertia condition uses axis acceleration as the metric.

If the number of FFCONDITION structures in the array is equal to the number of axes for the effect, the first structure applies to the first axis, the second applies to the second axis, and so on. For example, a two-axis spring condition with **lOffset** set to 0 in both FFCONDITION structures would have the same effect as the joystick self-centering spring. When a condition is defined for each axis in this way, the effect must not be rotated.

If there is a single FFCONDITION structure for an effect with more than one axis, the direction along which the parameters of the FFCONDITION structure are in effect is determined by the direction parameters passed in the **rglDirection** field of the FFEFFECT structure. For example, a friction condition rotated 45 degrees (in polar coordinates) would resist joystick motion in the northeast-southwest direction but would have no effect on joystick motion in the northwest-southeast direction.

## Topics

### Initializers

init()

init(lOffset: LONG, lPositiveCoefficient: LONG, lNegativeCoefficient: LONG, dwPositiveSaturation: DWORD, dwNegativeSaturation: DWORD, lDeadBand: LONG)

### Instance Properties

var dwNegativeSaturation: DWORD

Maximum force output on the negative side of the offset, in the range from 0 through 10,000.

var dwPositiveSaturation: DWORD

Maximum force output on the positive side of the offset, in the range from 0 through 10,000.

var lDeadBand: LONG

Region around **lOffset** in which the condition is not active, in the range from 0 through 10,000. In other words, the condition is not active between **lOffset** minus **lDeadBand** and **lOffset** plus **lDeadBand**.

var lNegativeCoefficient: LONG

Coefficient constant on the negative side of the offset, in the range from -10,000 through 10,000.

var lOffset: LONG

Offset for the condition, in the range from -10,000 through 10,000.

var lPositiveCoefficient: LONG

Coefficient constant on the positive side of the offset, in the range from -10,000 through 10,000.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Data Types

struct FFCAPABILITIES

Used by the FFDeviceGetForceFeedbackCapabilities method to retrieve device force-feedback capabilities.

struct FFCONSTANTFORCE

Contains type-specific information for the CONSTANTFORCE effect.

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

