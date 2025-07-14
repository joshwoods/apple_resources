

- HIDDriverKit
- IOUserUSBHostHIDDevice
-  newDeviceDescription 

Instance Method

# newDeviceDescription

Creates and returns a new dictionary that describes the HID device.

DriverKit 19.0+macOS

``` source
OSDictionary * newDeviceDescription();
```

## Return Value

An `OSDictionary` that describes the device.

## Discussion

This method uses the information from the USB device to create and return the dictionary of attributes. The dictionary always includes the following keys:

- kIOHIDReportIntervalKey

- kIOHIDVendorIDKey

- kIOHIDProductIDKey

- kIOHIDTransportKey

- kIOHIDVersionNumberKey

- kIOHIDCountryCodeKey

- `kIOHIDRequestTimeoutKey`

The dictionary may also contain some or all of the following keys:

- kIOHIDLocationIDKey

- kIOHIDManufacturerKey

- kIOHIDProductKey

- kIOHIDSerialNumberKey

