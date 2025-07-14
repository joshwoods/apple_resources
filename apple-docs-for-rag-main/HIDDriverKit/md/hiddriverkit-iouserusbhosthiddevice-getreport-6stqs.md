

- HIDDriverKit
- IOUserUSBHostHIDDevice
-  getReport 

Instance Method

# getReport

Gets a report from the HID device.

DriverKit 19.0+macOS

``` source
kern_return_t getReport(IOMemoryDescriptor * report, IOHIDReportType reportType, IOOptionBits options, uint32_t completionTimeout, OSAction * action);
```

## Parameters 

`report`  

A memory descriptor that contains the report from the HID device.

`reportType`  

The report type.

`options`  

The lower 8 bits of the report ID. The other 24 bits are options to specify the request.

`completionTimeout`  

The amount of time, in milliseconds, after which to abort the command if the entire command hasn’t completed.

`action`  

The function to call when the request completes. If you omit this function, the method executes synchronously, blocking the current thread until the request completes.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

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

