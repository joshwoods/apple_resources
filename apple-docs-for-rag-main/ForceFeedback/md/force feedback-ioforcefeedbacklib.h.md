

- Force Feedback
-  IOForceFeedbackLib.h 

API Collection

# IOForceFeedbackLib.h

Public Interfaces and constants used to develop Force Feedback plugIns.

## Overview

A force feedback device manufacturer might need to implement a plugIn to allow the Force Feedback Library to control the device. This header file describes the functions that need to be implemented. This interface definition follows Microsoft Windows IDirectInputEffectDriver definition wherever it makes sense to do so. This plugIn architecture uses the CFPlugIn model (COM). The Force Feedback Framework will find available plugIns and will use this interface to communicate with the hardware.

Certain functions may contain more or fewer parameters than the corresponding Windows IDirectInputEffectDriver version.

### Included Headers

- \

- \

- \

- \

- \

- \

## Topics

### Miscellaneous

DestroyEffect

This function commands the device to “destroy” a currently downloaded effect. The effect ID and any data that is associated with the effect are freed and available for reallocation.

DownloadEffect

This function sends an effect to the device.

Escape

This function escapes to the driver. This method is called in response to an application invoking the FFEffectEscape or FFDeviceEscape methods.

ForceFeedbackGetVersion

This function is used to determine driver and API version information.

GetEffectStatus

This function returns the device effect’s status.

GetForceFeedbackCapabilities

This function escapes to the driver. This method is called in response to an application invoking the FFEffectEscape or FFDevicEscape methods.

GetForceFeedbackState

This function returns the state of the device.

InitializeTerminate

This function is used to “create and destroy” particular device instances. It provides the FF plug-in driver with all the necessary start-up parameters.

SendForceFeedbackCommand

This function sends a command to the device.

SetProperty

This function sets properties that define the device behavior.

StartEffect

This function commands the device to play back an effect that was previously loaded.

StopEffect

This function commands the device to stop an effect that was previously started.

### Data Types

See the Overview for header-level documentation.

FFEffectDownloadID

Unique identification for an effect.

ForceFeedbackDeviceState

Returns information about the state of a force feedback device.

ForceFeedbackVersion

Used to return plugIn version information.

### Constants

Defines

## See Also

### Reference

ForceFeedback.h

Public Interfaces to the Force Feedback implementation in macOS.

ForceFeedbackConstants.h

Constants used in the public interfaces to the Force Feedback implementation in macOS.

ForceFeedback Structures

ForceFeedback Enumerations

ForceFeedback Data Types

