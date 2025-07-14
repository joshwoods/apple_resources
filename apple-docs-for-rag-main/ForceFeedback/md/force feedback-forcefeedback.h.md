

- Force Feedback
-  ForceFeedback.h 

API Collection

# ForceFeedback.h

Public Interfaces to the Force Feedback implementation in macOS.

## Overview

The Force Feedback API allows developers to control Force Feedback devices attached to the system. It is a distilled version of the Force Feedback functionality found in Microsoft’s DirectInput API. Developers familiar with that API should find this API to be similar.

### Included Headers

- \

- \

- \

- \

- \

## Topics

### Miscellaneous

func FFCreateDevice(io_service_t, UnsafeMutablePointer&lt;FFDeviceObjectReference?>!) -> HRESULT

Creates a new API device object from an OS object in preparation to use the device for force feedback.

func FFDeviceCreateEffect(FFDeviceObjectReference!, CFUUID!, UnsafeMutablePointer&lt;FFEFFECT>!, UnsafeMutablePointer&lt;FFEffectObjectReference?>!) -> HRESULT

Creates and initializes an instance of an effect identified by the effect UUID on the device.

func FFDeviceEscape(FFDeviceObjectReference!, UnsafeMutablePointer&lt;FFEFFESCAPE>!) -> HRESULT

Sends a hardware-specific command to the device.

func FFDeviceGetForceFeedbackCapabilities(FFDeviceObjectReference!, UnsafeMutablePointer&lt;FFCAPABILITIES>!) -> HRESULT

Retrieves the device’s force feedback capabilities.

func FFDeviceGetForceFeedbackProperty(FFDeviceObjectReference!, FFProperty, UnsafeMutableRawPointer!, IOByteCount) -> HRESULT

Gets properties that define the device behavior.

func FFDeviceGetForceFeedbackState(FFDeviceObjectReference!, UnsafeMutablePointer&lt;FFState>!) -> HRESULT

Retrieves the state of the device’s force feedback system.

func FFDeviceReleaseEffect(FFDeviceObjectReference!, FFEffectObjectReference!) -> HRESULT

Disposes of an API effect object created with FFDeviceCreateEffect.

func FFDeviceSendForceFeedbackCommand(FFDeviceObjectReference!, FFCommandFlag) -> HRESULT

Sends a command to the device’s force feedback system.

func FFDeviceSetCooperativeLevel(FFDeviceObjectReference!, UnsafeMutableRawPointer!, FFCooperativeLevelFlag) -> HRESULT

Function is unimplemented in version 1.0 of this API

func FFDeviceSetForceFeedbackProperty(FFDeviceObjectReference!, FFProperty, UnsafeMutableRawPointer!) -> HRESULT

Retrieves the device’s force feedback capabilities.

func FFEffectDownload(FFEffectObjectReference!) -> HRESULT

Places the effect on the device. If the effect is already on the device, the existing effect is updated to match the values set by the FFEffectSetParameters method.

func FFEffectEscape(FFEffectObjectReference!, UnsafeMutablePointer&lt;FFEFFESCAPE>!) -> HRESULT

Sends a hardware-specific command to the driver.

func FFEffectGetEffectStatus(FFEffectObjectReference!, UnsafeMutablePointer&lt;FFEffectStatusFlag>!) -> HRESULT

Sends a hardware-specific command to the driver.

func FFEffectGetParameters(FFEffectObjectReference!, UnsafeMutablePointer&lt;FFEFFECT>!, FFEffectParameterFlag) -> HRESULT

Retrieves information about an effect.

func FFEffectSetParameters(FFEffectObjectReference!, UnsafeMutablePointer&lt;FFEFFECT>!, FFEffectParameterFlag) -> HRESULT

Sets the characteristics of an effect.

func FFEffectStart(FFEffectObjectReference!, UInt32, FFEffectStartFlag) -> HRESULT

Begins playing an effect. If the effect is already playing, it is restarted from the beginning. If the effect has not been downloaded or has been modified since its last download, it is downloaded before being started. This default behavior can be suppressed by passing the FFES_NODOWNLOAD flag.

func FFEffectStop(FFEffectObjectReference!) -> HRESULT

Stops playing an effect.

func FFEffectUnload(FFEffectObjectReference!) -> HRESULT

Removes the effect from the device. If the effect is playing, it is automatically stopped before it is unloaded.

func FFIsForceFeedback(io_service_t) -> HRESULT

Used to determine if a particular device provided by HID Manager is a force feedback device.

func FFReleaseDevice(FFDeviceObjectReference!) -> HRESULT

Disposes of an API device object created with FFCreateDevice.

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

struct FFENVELOPE

Used by the FFEFFECT structure to specify the optional envelope parameters for an effect.

struct FFPERIODIC

A structure containing type-specific information for certain effects.

struct FFRAMPFORCE

Contains type-specific information for the RAMPFORCE effect.

## See Also

### Reference

ForceFeedbackConstants.h

Constants used in the public interfaces to the Force Feedback implementation in macOS.

ForceFeedback Enumerations

ForceFeedback Constants

ForceFeedback Data Types

