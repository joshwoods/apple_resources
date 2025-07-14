

- Kernel
- Deprecated Symbols
- IOUSBInterface
-  GetEndpointProperties 

# GetEndpointProperties

Returns the properties of an endpoint, possibly in an alternate interface.

``` source
virtual IOReturn GetEndpointProperties(
 UInt8alternateSetting,
 UInt8endpointNumber,
 UInt8direction,
 UInt8 *transferType,
 UInt16 *maxPacketSize,
 UInt8 *interval); 
```

## Parameters 

`alternateSetting`  

specifies the desired alternate setting

`endpointNumber`  

specifies the endpoint number

`direction`  

specifies the direction (kUSBIn, kUSBOut)

`transferType`  

a pointer to hold the transfer type (kUSBControl, kUSBBulk, etc.) of the endpoint if found.

`maxPacketSize`  

a pointer to hold the maxPacketSize in the endpoint descriptor.

`interval`  

a pointer to hold the interval value in the endpoint descriptor.

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

