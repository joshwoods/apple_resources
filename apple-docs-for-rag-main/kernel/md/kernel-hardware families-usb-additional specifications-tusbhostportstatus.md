

- Kernel
- Hardware Families
- USB
- Additional Specifications
-  tUSBHostPortStatus 

# tUSBHostPortStatus

Constants for the USB host port status.

macOS 10.11+

``` source
enum tUSBHostPortStatus : unsigned int {
    ...
};
```

## Topics

### Constants

kUSBHostPortStatusConnectedSpeedFull

The full connected speed.

kUSBHostPortStatusConnectedSpeedHigh

The high connected speed.

kUSBHostPortStatusConnectedSpeedLow

The low connected speed.

kUSBHostPortStatusConnectedSpeedMask

The connected speed mask.

kUSBHostPortStatusConnectedSpeedNone

No connected speed.

kUSBHostPortStatusConnectedSpeedPhase

The connected speed phase.

kUSBHostPortStatusConnectedSpeedSuper

The SuperSpeed connected speed.

kUSBHostPortStatusEnabled

The port status enabled value.

kUSBHostPortStatusOvercurrent

The port status overcurrent.

kUSBHostPortStatusPortTypeAccessory

The accessory port type.

kUSBHostPortStatusPortTypeCaptive

The captive port type.

kUSBHostPortStatusPortTypeInternal

The internal port type.

kUSBHostPortStatusPortTypeMask

The port type mask.

kUSBHostPortStatusPortTypePhase

The port type phase.

kUSBHostPortStatusPortTypeReserved

The reserved port type.

kUSBHostPortStatusPortTypeStandard

The standard port type.

kUSBHostPortStatusResetting

The resetting port status.

kUSBHostPortStatusSuspended

The suspended port status.

kUSBHostPortStatusTestMode

The test mode port status.

kUSBHostPortStatusConnectedSpeedSuperPlus

The SuperSpeedPlus connected speed.

kUSBHostPortStatusConnectedSpeedSuperPlusBy2

The SuperSpeedPlus By 2 connected speed.

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

USBDeviceInformationBits

The state of a USB device.

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

