

- HIDDriverKit
- IOUserUSBHostHIDDevice
-  getReport 

Instance Method

# getReport

Gets a report from the HID device.

DriverKit 19.0+macOS

``` source
kern_return_t getReport(IOMemoryDescriptor * report, IOHIDReportType reportType, IOOptionBits options, uint32_t completionTimeout, uint32_t * bytesTransferred);
```

## Parameters 

`report`  

The report type.

`reportType`  

The lower 8 bits will represent the Report ID. The other 24 bits are options to specify the request.

`options`  

Specifies an amount of time (in ms) after which the command will be aborted if the entire command has not been completed.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

The report read from the HID device.

## See Also

### Managing Device Reports

newReportDescriptor

Returns the data in the HID device’s report descriptor.

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

