

- Kernel
- Deprecated Symbols
- IOUSBInterface
-  FindNextAltInterface 

# FindNextAltInterface

``` source
virtual const IOUSBInterfaceDescriptor *FindNextAltInterface(
 const IOUSBInterfaceDescriptor *current, 
 IOUSBFindInterfaceRequest *request); 
```

## Parameters 

`current`  

interface descriptor to start searching from, NULL to start at alternate interface 0.

`request`  

specifies what properties an interface must have to match.

## Return Value

Pointer to a matching interface descriptor, or NULL if none match.

## Overview

return alternate interface descriptor satisfying the requirements specified in request, or NULL if there aren't any. request is updated with the properties of the returned interface.

## See Also

### Miscellaneous

DeviceRequest(IOUSBDevRequest *, IOUSBCompletion *)

Sends a control request to the default control pipe in the device (pipe zero)

DeviceRequest(IOUSBDevRequestDesc *, IOUSBCompletion *)

Sends a control request to the default control pipe in the device (pipe zero)

EnableRemoteWake

Will enable or disable the USB 3.0 remote wake function for the interface

FindNextAssociatedDescriptor

FindNextPipe(IOUSBPipe *, IOUSBFindEndpointRequest *)

FindNextPipe(IOUSBPipe *, IOUSBFindEndpointRequest *, bool)

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

