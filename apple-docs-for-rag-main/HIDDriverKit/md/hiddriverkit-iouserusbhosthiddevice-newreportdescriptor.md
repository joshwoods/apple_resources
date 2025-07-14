

- HIDDriverKit
- IOUserUSBHostHIDDevice
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

The default implementation of this method fetches the report descriptor from the USB device and packages the resulting data into an OSData object.

## See Also

### Managing Device Reports

getReport

Gets a report from the HID device.

getReport

Gets a report from the HID device.

setReport

Sends a report to the HID device.

initInputReport

Starts reading the input report from the device.

CompleteInputReport

Processes the results of an asynchronous request for an input report.

scheduleInputReportRetry

Retries a previous request for an input report.

cancelInputReportRetry

Cancels a retry attempt for an input report request.

TimerOccurred

Handles timeout-related actions when retrying input report requests.

