

- Kernel
- Deprecated Symbols
- IOUSBInterface
-  DeviceRequest(IOUSBDevRequest \*, IOUSBCompletion \*) 

# DeviceRequest(IOUSBDevRequest \*, IOUSBCompletion \*)

Sends a control request to the default control pipe in the device (pipe zero)

``` source
virtual IOReturn DeviceRequest(
 IOUSBDevRequest *request,
 IOUSBCompletion *completion = 0); 
```

## Parameters 

`request`  

The parameter block to send to the device

`completion`  

Function to call when request completes. If omitted then DeviceRequest() executes synchronously, blocking until the request is complete. If the request is asynchronous, the client must make sure that the IOUSBDevRequest is not released until the callback has occurred.

## See Also

### Miscellaneous

DeviceRequest(IOUSBDevRequestDesc *, IOUSBCompletion *)

Sends a control request to the default control pipe in the device (pipe zero)

EnableRemoteWake

Will enable or disable the USB 3.0 remote wake function for the interface

FindNextAltInterface

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

