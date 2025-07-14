

- USBDriverKit
-  tIOUSBDeviceRequest 

Enumeration

# tIOUSBDeviceRequest

Constants for configuring a device request.

DriverKit 19.0+

``` source
enum tIOUSBDeviceRequest : unsigned int;
```

## Topics

### Getting the Device Request Settings

kIOUSBDeviceRequestSize

kIOUSBDeviceRequestDirectionMask

kIOUSBDeviceRequestDirectionPhase

kIOUSBDeviceRequestDirectionOut

kIOUSBDeviceRequestDirectionIn

kIOUSBDeviceRequestTypeMask

kIOUSBDeviceRequestTypePhase

kIOUSBDeviceRequestTypeStandard

kIOUSBDeviceRequestTypeClass

kIOUSBDeviceRequestTypeVendor

kIOUSBDeviceRequestRecipientMask

kIOUSBDeviceRequestRecipientPhase

kIOUSBDeviceRequestRecipientDevice

kIOUSBDeviceRequestRecipientInterface

kIOUSBDeviceRequestRecipientEndpoint

kIOUSBDeviceRequestRecipientOther

## See Also

### Device Requests

Standard Device Requests

Constants for the standard requests you can make to a USB device.

IOUSBDeviceRequest

A structure that defines a standard device request.

IOUSBDeviceRequestSetSELData

The structure for receiving system exit latency values.

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

