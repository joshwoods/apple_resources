

- Kernel
- Deprecated Symbols
- IOUSBInterface
-  GetEndpointPropertiesV3 

# GetEndpointPropertiesV3

Returns the properties of an endpoint, possibly in an alternate interface, including any information from the SuperSpeed Companion Descriptor

``` source
virtual IOReturn GetEndpointPropertiesV3(
 IOUSBEndpointProperties *endpointProperties); 
```

## Parameters 

`endpointProperties`  

Pointer to a IOUSBEndpointProperties structure that upon success will contain the information for the endpoint. The bVersion field needs to be initialized with the structure version (see USBEndpointVersion enum in USB.h). The bAlternateSetting, bEndpointNumber, and bDirection (kUSBIn, kUSBOut) MUST also be filled in with the values for the desired descriptor. Not that the bMaxStreams value for Bulk endpoints is the value specified by the bmAttributes field in the SuperSpeed companion descriptor.

## Return Value

returns kIOReturnSuccess if the endpoint is found, and kIOUSBEndpointNotFound if it is not.

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

