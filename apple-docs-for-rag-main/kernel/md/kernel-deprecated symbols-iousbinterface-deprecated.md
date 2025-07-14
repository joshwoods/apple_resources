

- Kernel
- Deprecated Symbols
-  IOUSBInterface Deprecated

Class

# IOUSBInterface

An object that represents an interface of a device on the USB bus.

macOS 10.0–10.10Deprecated

``` source
class IOUSBInterface : IOService
```

Deprecated

Use IOUSBHostInterface instead.

## Overview

Use this class to find an interface’s pipes and read its associated descriptors.

## Topics

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

SetFunctionSuspendFeature

Issues a SET_FEATURE(FUNCTION_SUSPEND) to the interface.

### Instance Methods

- getMetaClass

## Relationships

### Inherits From

- IOService

## See Also

### IOKit

IOUSBDevice

An input/output service object that represents a device on the USB bus.

Deprecated

IOOFPathMatchingDeprecated

IOUSBHostInterfaceDeprecated

IOUSBHostDeviceDeprecated

IOUSBHostPipeDeprecated

IOUSBHostIOSourceDeprecated

IOUSBHostStreamDeprecated

IOHIDEventDriverDeprecated

IOHIDEventService

IOService represents an device or OS service in IOKit and DriverKit.

Deprecated

IOHIDInterface

IOService represents an device or OS service in IOKit and DriverKit.

Deprecated

IOHIDSystemDeprecated

IOHIKeyboardMapperDeprecated

IOHIKeyboardDeprecated

IOHIPointingDeprecated

IOHIDeviceDeprecated

IOHIDElementDeprecated

IOHIDWorkLoopDeprecated

IOEthernetInterface

The Ethernet interface object.

Deprecated

IOEthernetController

Abstract superclass for Ethernet controllers.

Deprecated

