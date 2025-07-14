

- Force Feedback
- IOForceFeedbackLib.h
-  Escape 

Article

# Escape

This function escapes to the driver. This method is called in response to an application invoking the FFEffectEscape or FFDeviceEscape methods.

## Overview

```
HRESULT ( *Escape)(
   void *self,
   FFEffectDownloadID downloadID,
   FFEFFESCAPE *pEscape );
```

### Parameters

self  
Pointer to the FFPlugInDriver implementation instance.

downloadID  
Specifies the effect at which the command is directed, or zero if the command is directed at the device itself and not any particular effect.

pEscape  
Pointer to a FFEFFESCAPE structure that describes the command to be sent. On success, the cbOutBuffer member contains the number of output buffer bytes actually used.

### Return Value

Returns FF_OK if successful, or an error value otherwise:

FFERR_UNSUPPORTED

## See Also

### Miscellaneous

DestroyEffect

This function commands the device to “destroy” a currently downloaded effect. The effect ID and any data that is associated with the effect are freed and available for reallocation.

DownloadEffect

This function sends an effect to the device.

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

