

- USBDriverKit
-  IOUSBDeviceRequestSetSELData 

Structure

# IOUSBDeviceRequestSetSELData

The structure for receiving system exit latency values.

DriverKit 19.0+

``` source
struct IOUSBDeviceRequestSetSELData;
```

## Overview

For information about the `Set SEL` request type, see section 9.4.12 of the USB 3.0 specification at http://www.usb.org.

## Topics

### Getting the SEL Data

u1Sel

u1Pel

u2Sel

u2Pel

## See Also

### Device Requests

Standard Device Requests

Constants for the standard requests you can make to a USB device.

IOUSBDeviceRequest

A structure that defines a standard device request.

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

