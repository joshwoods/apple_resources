

- Force Feedback
-  FFCAPABILITIES 

Structure

# FFCAPABILITIES

Used by the FFDeviceGetForceFeedbackCapabilities method to retrieve device force-feedback capabilities.

Mac Catalyst 13.0+macOS 10.2+

``` source
struct FFCAPABILITIES
```

## Overview

This structure has no DirectInput equivalent.

## Topics

### Initializers

init()

init(ffSpecVer: NumVersion, supportedEffects: UInt32, emulatedEffects: UInt32, subType: UInt32, numFfAxes: UInt32, ffAxes: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8), storageCapacity: UInt32, playbackCapacity: UInt32, firmwareVer: NumVersion, hardwareVer: NumVersion, driverVer: NumVersion)

### Instance Properties

var driverVer: NumVersion

Specifies the version number of the force-feedback device driver, using a NumVersion structure.

var emulatedEffects: UInt32

FFCapabilitiesEffectType flags that identify all effect types not directly supported by the device, but emulated by the plugIn.

var ffAxes: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)

An array of values that describe the axes on which force-feedback is present.

var ffSpecVer: NumVersion

Specifies the version number of the FF API specification supported by this plugIn. It should be specified using the fields of the NumVersion structure. The first version of the FF API specification is 1.0.0f0.

var firmwareVer: NumVersion

Specifies the firmware revision of the device, using a NumVersion structure.

var hardwareVer: NumVersion

Specifies the hardware revision of the device, using a NumVersion structure.

var numFfAxes: UInt32

The number of controller axes that provide force feedback. Indicates the number of valid elements in ffAxes.

var playbackCapacity: UInt32

The maximum number of created effects that can be simultaneously played via calls to FFEffectStart. This number will always be equal to or less than the storageCapacity. A device driver may allow more effects to be created than the physical device can actually handle. Therefore, this number is an important parameter for FF designers.

var storageCapacity: UInt32

The maximum number of effects that can be created via calls to FFDeviceCreateEffect and coexist at any one time. This may or may not be different from the playbackCapacity, depending on device driver complexity.

var subType: UInt32

The force-feedback subcategory which best identifies the device’s FF capabilities.

var supportedEffects: UInt32

FFCapabilitiesEffectType flags that identify all effect types supported by the plugIn/device (including driver-emulated effects).

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Data Types

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

struct FFENVELOPE

Used by the FFEFFECT structure to specify the optional envelope parameters for an effect.

struct FFPERIODIC

A structure containing type-specific information for certain effects.

struct FFRAMPFORCE

Contains type-specific information for the RAMPFORCE effect.

