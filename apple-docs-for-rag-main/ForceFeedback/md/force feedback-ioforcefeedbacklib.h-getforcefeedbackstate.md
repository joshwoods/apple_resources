

- Force Feedback
- IOForceFeedbackLib.h
-  GetForceFeedbackState 

Article

# GetForceFeedbackState

This function returns the state of the device.

## Overview

```
HRESULT ( *GetForceFeedbackState)(
   void *self,
   ForceFeedbackDeviceState *pDeviceState );
```

### Parameters

self  
Pointer to the FFPlugInDriver implementation instance.

pDeviceState  
Pointer to a ForceFeedbackDeviceState structure that receives the device state. FF API sets the dwSize member of the ForceFeedbackDeviceState structure to sizeof(ForceFeedbackDeviceState) before calling this method.

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

GetEffectStatus

This function returns the device effect’s status.

GetForceFeedbackCapabilities

This function escapes to the driver. This method is called in response to an application invoking the FFEffectEscape or FFDevicEscape methods.

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

