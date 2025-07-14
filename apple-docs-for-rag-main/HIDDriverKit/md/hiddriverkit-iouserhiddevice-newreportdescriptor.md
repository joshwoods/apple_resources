

- HIDDriverKit
- IOUserHIDDevice
-  newReportDescriptor 

Instance Method

# newReportDescriptor

Returns the data in the HID device’s report descriptor.

DriverKit 19.0+macOS

``` source
OSData * newReportDescriptor();
```

## Return Value

An OSData object containing the report descriptor for the device.

## Discussion

Override this method and use it to fetch the report descriptor from the device. Return the raw bytes for that report in an OSData object.

