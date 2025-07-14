

- Force Feedback
- IOForceFeedbackLib.h
-  GetEffectStatus 

Article

# GetEffectStatus

This function returns the device effect’s status.

## Overview

```
HRESULT ( *GetEffectStatus)(
   void *self,
   FFEffectDownloadID downloadID,
   FFEffectStatusFlag *pStatusCode );
```

### Parameters

self  
Pointer to the FFPlugInDriver implementation instance.

downloadID  
Indicates the effect to be queried.

pStatusCode  
Receives the effect status. The FFEffectStatusFlag pointed to by this parameter should be filled in with one of the following values:

FFEGES_PLAYING

The effect is still playing.

FFEGES_NOTPLAYING

The effect is not playing.

### Return Value

Returns FF_OK.

## See Also

### Miscellaneous

DestroyEffect

This function commands the device to “destroy” a currently downloaded effect. The effect ID and any data that is associated with the effect are freed and available for reallocation.

DownloadEffect

This function sends an effect to the device.

Escape

This function escapes to the driver. This method is called in response to an application invoking the FFEffectEscape or FFDeviceEscape methods.

ForceFeedbackGetVersion

This function is used to determine driver and API version information.

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

