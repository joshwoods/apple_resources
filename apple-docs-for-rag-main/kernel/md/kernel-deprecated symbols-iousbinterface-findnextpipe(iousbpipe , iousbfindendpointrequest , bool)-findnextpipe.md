

- Kernel
- Deprecated Symbols
- IOUSBInterface
-  FindNextPipe(IOUSBPipe \*, IOUSBFindEndpointRequest \*, bool) 

# FindNextPipe(IOUSBPipe \*, IOUSBFindEndpointRequest \*, bool)

``` source
virtual IOUSBPipe* FindNextPipe(
 IOUSBPipe *current,
 IOUSBFindEndpointRequest *request,
 boolwithRetain); 
```

## Parameters 

`current`  

Pipe to start searching from, NULL to start from beginning of list.

`request`  

Requirements for pipe to match, updated with the found pipe's properties.

`withRetain`  

Pass true to retain and the client should release it later after its use.

## Return Value

Pointer to the pipe, or NULL if no pipe matches the request.

## Overview

Find a pipe of the interface that matches the requirements, either starting from the beginning of the interface's pipe list or from a specified pipe.

## See Also

### Miscellaneous

DeviceRequest(IOUSBDevRequest *, IOUSBCompletion *)

Sends a control request to the default control pipe in the device (pipe zero)

DeviceRequest(IOUSBDevRequestDesc *, IOUSBCompletion *)

Sends a control request to the default control pipe in the device (pipe zero)

EnableRemoteWake

Will enable or disable the USB 3.0 remote wake function for the interface

FindNextAltInterface

FindNextAssociatedDescriptor

FindNextPipe(IOUSBPipe *, IOUSBFindEndpointRequest *)

GetAlternateSetting

GetConfigValue

GetDevice

GetEndpointProperties

Returns the properties of an endpoint, possibly in an alternate interface.

GetEndpointPropertiesV3

Returns the properties of an endpoint, possibly in an alternate interface, including any information from the SuperSpeed Companion Descriptor

GetInterfaceClass

GetInterfaceNumber

GetInterfaceProtocol

GetInterfaceStatus

Returns the result of issuing a GET_STATUS request on the device for this interface.

GetInterfaceStringIndex

GetInterfaceSubClass

GetNumEndpoints

GetPipeObj

RecreateStreams

RememberStreams

RememberStreams.

SetAlternateInterface

SetFunctionSuspendFeature

Issues a SET_FEATURE(FUNCTION_SUSPEND) to the interface.

