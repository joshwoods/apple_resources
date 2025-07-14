

- Kernel
- Hardware Families
- USB
- Additional Specifications
-  tIOUSB30LinkStateTimeout 

# tIOUSB30LinkStateTimeout

Constants for the link state timeout values on USB 3.0 devices.

macOS 10.15+

``` source
enum tIOUSB30LinkStateTimeout : unsigned int {
    ...
};
```

## Discussion

For information about these constants, see USB 3.2, 7.5, 7.5.4, 7.5.9, and 7.5.10.

## Topics

### Constants

kIOUSB30LinKStateU2RxDetectDelay

The USB 2.0 receive detect delay.

kIOUSB30LinkStateHotResetActiveTimeout

The hot reset active timeout.

kIOUSB30LinkStateLoopbackExitTimeout

The loopback exit timeout.

kIOUSB30LinkStatePollingActiveTimeout

The polling active timeout.

kIOUSB30LinkStatePollingConfigurationTimeout

The polling configuration timeout.

kIOUSB30LinkStatePollingDeadline

The polling deadline.

kIOUSB30LinkStatePollingIdleTimeout

The polling idle timeout.

kIOUSB30LinkStatePollingLFPSTimeout

The polling LFPS timeout.

kIOUSB30LinkStateRecoveryActiveTimeout

The recovery active timeout.

kIOUSB30LinkStateRecoveryConfigurationTimeout

The recovery configuration timeout.

kIOUSB30LinkStateRecoveryIdleTimeout

The recovery idle timeout.

kIOUSB30LinkStateRxDetectQuietTimeout

The receive detect quiet timeout.

kIOUSB30LinkStateSSInactiveQuietTimeout

The SuperSpeed inactive quiet timeout.

kIOUSB30LinkStateSSResumeDeadline

The SuperSpeed resume deadline.

kIOUSB30LinkStateU0LTimeout

The U0L timeout.

kIOUSB30LinkStateU0RecoveryTimeout

The U0 recovery timeout.

kIOUSB30LinkStateU1NoLFPSResponseTimeout

The U1 no LFPS response timeout.

kIOUSB30LinkStateU1PingTimeout

The U1 ping timeout.

kIOUSB30LinkStateU2NoLFPSResponseTimeout

The U2 no LFPS response timeout.

kIOUSB30LinkStateU3NoLFPSResponseTimeout

The U3 no LFPS response timeout.

kIOUSB30LinkStateU3RxDetectDelay

The U3 receive detect delay.

kIOUSB30LinkStateU3WakeupRetryDelay

The U3 wakeup retry delay.

kIOUSB30LinkStateHotResetDeadline

kIOUSB30LinkStateHotResetExitTimeout

kIOUSB30LinkStateRecoveryDeadline

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

