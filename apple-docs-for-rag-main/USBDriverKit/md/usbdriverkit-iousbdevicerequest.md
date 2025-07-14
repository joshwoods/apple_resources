

- USBDriverKit
-  IOUSBDeviceRequest 

Structure

# IOUSBDeviceRequest

A structure that defines a standard device request.

DriverKit 19.0+

``` source
struct IOUSBDeviceRequest;
```

## Overview

For information about device requests, see section 9.3 of the USB 2.0 specification at http://www.usb.org.

## Topics

### Getting the Request Data

bmRequestType

bRequest

wValue

wIndex

wLength

## See Also

### Device Requests

Standard Device Requests

Constants for the standard requests you can make to a USB device.

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

