

- Kernel
- Deprecated Symbols
- IOUSBInterface
-  SetFunctionSuspendFeature 

# SetFunctionSuspendFeature

Issues a SET_FEATURE(FUNCTION_SUSPEND) to the interface.

``` source
virtual IOReturn SetFunctionSuspendFeature(
 UInt8options); 
```

## Parameters 

`options`  

The suspend options passed to the Device Request.

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

