

- Kernel
- Hardware Families
- USB
- Additional Specifications
-  USBDeviceInformationBits 

Type Alias

# USBDeviceInformationBits

The state of a USB device.

macOS 10.6+

``` source
typedef enum USBDeviceInformationBits USBDeviceInformationBits;
```

## Discussion

GetUSBDeviceInformation returns a `unit32_t` value with bits set indicating that a particular state is present in the USB device.

## Topics

### Constants

kUSBInformationDeviceIsCaptiveBit

The USB device has directly attached to its hub and isn’t removable.

kUSBInformationDeviceIsAttachedToRootHubBit

The USB device has directly attached to the root hub.

kUSBInformationDeviceIsInternalBit

The USB device is internal to the enclosure.

kUSBInformationDeviceIsConnectedBit

The system has connected the USB device to its hub.

kUSBInformationDeviceIsEnabledBit

The system has enabled the hub port that the USB device attaches to.

kUSBInformationDeviceIsSuspendedBit

The system has suspended the hub port that the USB device attaches to.

kUSBInformationDeviceIsInResetBit

The system is resetting the hub port that the USB attaches to.

kUSBInformationDeviceOvercurrentBit

The USB device generated an overcurrent.

kUSBInformationDevicePortIsInTestModeBit

The hub port that the USB device attaches to is in test mode.

kUSBInformationDeviceIsRootHub

The device is the root hub simulation.

kUSBInformationRootHubisBuiltIn

The USB root hub is built-in.

kUSBInformationDeviceIsRemote

This device attaches to the controller through a remote connection.

kUSBInformationDeviceIsAttachedToEnclosure

The hub port that the USB device connects to has a USB connector on the enclosure.

kUSBInformationDeviceIsOnThunderbolt

The USB device is downstream of a controller that attaches through a Thunderbolt port.

kUSBInformationDeviceIsAttachedToEnclosureMask

The mask indicating that the USB device has attached to an enclosure.

kUSBInformationDeviceIsAttachedToRootHubMask

The mask indicating that the USB device has attached to a root hub.

kUSBInformationDeviceIsCaptiveMask

The mask indicating that the USB device is captive.

kUSBInformationDeviceIsConnectedMask

The mask indicating that the USB device has connected.

kUSBInformationDeviceIsEnabledMask

The mask indicating that the USB device is in an enabled state.

kUSBInformationDeviceIsInResetMask

The mask indicating that the USB device is in a reset state.

kUSBInformationDeviceIsInternalMask

The mask indicating that the USB device is internal.

kUSBInformationDeviceIsOnThunderboltBit

The bit indicating that the USB device is on a Thunderbolt port.

kUSBInformationDeviceIsOnThunderboltMask

The mask indicating that the USB device is on a Thunderbolt port.

kUSBInformationDeviceIsRemoteMask

The mask indicating that the USB device is remote.

kUSBInformationDeviceIsRootHubMask

The mask indicating that the USB device is a root hub.

kUSBInformationDeviceIsSuspendedMask

The mask indicating that the USB device is in a suspended state.

kUSBInformationDeviceOvercurrentMask

The mask indicating that the USB device is in overcurrent.

kUSBInformationDevicePortIsInTestModeMask

The mask indicating that the USB device is in test mode.

kUSBInformationRootHubIsBuiltInBit

The bit indicating that the root hub is built-in.

kUSBInformationRootHubIsBuiltInMask

The mask indicating that the root hub is built-in.

kUSBInformationRootHubisBuiltInMask

The mask indicating that the root hub is built-in.

## See Also

### USB Types

tIOUSB20BusCurrent

Constants for the available current levels for USB 2.0 devices.

tIOUSB30BusCurrent

Constants for the available power levels of USB 3.0 devices.

tIOUSB30DeviceNotificationType

Constants indicating the type of a device notification.

tIOUSB30HubExtStatus

Bit masks for getting port status values.

tIOUSB30HubPortStatusCode

Constants for the port status type codes.

tIOUSB30LinkStateTimeout

Constants for the link state timeout values on USB 3.0 devices.

tIOUSB30ResetTimeout

Constants for the reset timeout values on USB 3.0 devices.

tIOUSB30TimingParameters

Constants for USB 3.0 timing parameters.

tIOUSBBusVoltage

A constant for the USB bus voltage.

tIOUSBDeviceCapabilityType

Constants for the device capability types.

tIOUSBDeviceRequest

Constants for configuring a device request.

tIOUSBDeviceRequestDirectionValue

Enumerated device request direction values.

tIOUSBDeviceRequestRecipientValue

Constants indicating the type of object that receives the results of a request.

tIOUSBDeviceRequestTypeValue

Constants indicating the type of request to make from a device.

tIOUSBEndpointDirection

The direction of data transfers on an endpoint.

tIOUSBEndpointSynchronizationType

Constants for the endpoint synchronization types.

tIOUSBEndpointType

Constants describing the types of endpoints.

tIOUSBEndpointUsageType

Constants for the endpoint usage types.

tIOUSBHostConnectionSpeed

Constants indicating the connection speed of the device.

tIOUSBHostPortStatus

Constants indicating the state of a port.

tIOUSBHostPortType

Constants indicating a port’s type.

tIOUSBLanguageID

Constants for the USB language identifiers.

tInternalUSBHostConnectionSpeed

Constants for the internal USB host connection speed.

tUSBHostConnectionSpeed

Constants for the USB host connection speed.

tUSBHostDeviceAddress

The USB host device address.

tUSBHostPortStatus

Constants for the USB host port status.

tUSBHostPortType

Constants for the USB host port type.

IOUSBGetFrameStruct

A structure that contains frame information.

IOUSBHostIOSourceClientRecord

The USB host input/output source client record.

IOUSBIsocFrame

A structure for encoding information about a single frame in an isochronous transfer.

IOUSBIsocStruct

An internal structure to pass parameters between IOUSBLib and UserClient.

IOUSBLowLatencyIsocFrame

A structure for encoding information about each low-latency isochronous frame.

IOUSBLowLatencyIsocStruct

An internal structure to pass parameters between IOUSBLib and UserClient.

IOUSBKeyboardData

A structure containing USB keyboard data.

IOUSBKeyboardDataPtr

A pointer to a structure containing USB keyboard data.

IOUSBMouseData

A structure containing USB mouse data.

IOUSBMouseDataPtr

A pointer to a structure containing USB mouse data.

IOUSBMatch

A structure for matching USB devices.

USBClassSpecificDesc

A class-specific descriptor.

USBDeviceAddress

A USB device address.

USBHubClassRequest

A structure that provides USB hub requests.

USBLowLatencyBufferType

Specifies which kind of low-latency buffer to create.

USBNotificationTypes

Defines types of USB notifications.

USBPhysicalAddress32

A 32-bit USB physical address.

USBPowerRequestTypes

Specifies the kind of power to reserve.

USBReEnumerateOptions

Options for reenumerating a device.

USBStatus

The value of the USB device status.

USBStatusPtr

A pointer to a USB status.

