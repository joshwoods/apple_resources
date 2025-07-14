

- USBDriverKit
-  Additional Specifications 

API Collection

# Additional Specifications

Request information from a device and get hardware and timing information.

## Topics

### Device Requests

Standard Device Requests

Constants for the standard requests you can make to a USB device.

IOUSBDeviceRequest

A structure that defines a standard device request.

IOUSBDeviceRequestSetSELData

The structure for receiving system exit latency values.

tIOUSBDeviceRequest

Constants for configuring a device request.

tIOUSBDeviceRequestTypeValue

Constants indicating the type of request to make from a device.

tIOUSBDeviceRequestRecipientValue

Constants indicating the type of object that receives the results of a request.

Get Status Options

Constants for use with get status requests.

Suspend Feature Options

Constants to use when enabling the suspend feature of a device.

Link Power Management Capabilities

Constants for link power management capabilities.

Standard Feature Selectors

Constants for the standard feature selectors.

### Hub Port Status Requests

IOUSB30HubPortStatusExt

The structure for getting the port status of a USB 3 hub.

tIOUSBDeviceRequestDirectionValue

Enumerated device request direction values.

tIOUSB30HubExtStatus

Bit masks for getting port status values.

tIOUSB30HubPortStatusCode

Constants for the port status type codes.

Hub Parameters

Constants for hub parameters.

### Device Notifications

tIOUSB30DeviceNotificationType

Constants indicating the type of a device notification.

### Electrical Characteristics

tIOUSB20BusCurrent

Constants for the available current levels for USB 2.0 devices.

tIOUSB30BusCurrent

Constants for the available power levels of USB 3.0 devices.

tIOUSBBusVoltage

A constant for the USB bus voltage.

### Timing Parameters

tIOUSB30LinkStateTimeout

Constants for the link state timeout values on USB 3.0 devices.

tIOUSB30ResetTimeout

Constants for the reset timeout values on USB 3.0 devices.

tIOUSB30TimingParameters

Constants for USB 3.0 timing parameters.

Timing Parameters

Constants for ping response times.

## See Also

### USB Specifications

USB Device Descriptors

Determine the capabilities and configuration of a device using descriptors from the USB specification.

Registry Property Names

Search for specific keys in the device registry.

Utilities

Manipulate bit structures and convert integers between device- and platform-native formats.

