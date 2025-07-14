

- Kernel
- Deprecated Symbols
- IOUSBInterface
-  GetInterfaceStatus 

# GetInterfaceStatus

Returns the result of issuing a GET_STATUS request on the device for this interface.

``` source
virtual IOReturn GetInterfaceStatus(
 USBStatus *status); 
```

## Parameters 

`status`  

Pointer to a USBStatus type which will contain the results of the operation.

## Return Value

returns kIOReturnSuccess if the request is completed successfully, otherwise returns the result of the Device Request.

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

