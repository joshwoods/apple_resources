

- HIDDriverKit
- IOUserHIDDevice
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

Override this method and return a dictionary of key-value pairs that describe the device. The supported keys are:

- kIOHIDReportIntervalKey

- kIOHIDVendorIDKey

- kIOHIDProductIDKey

- kIOHIDTransportKey

- kIOHIDVersionNumberKey

- kIOHIDCountryCodeKey

- kIOHIDLocationIDKey

- kIOHIDManufacturerKey

- kIOHIDProductKey

- kIOHIDSerialNumberKey

- `kIOHIDRequestTimeoutKey`

