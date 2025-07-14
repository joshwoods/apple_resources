

- HIDDriverKit
- IOUserUSBHostHIDDevice
-  CompleteInputReport 

Instance Method

# CompleteInputReport

Processes the results of an asynchronous request for an input report.

DriverKit 19.0+macOS

``` source
void CompleteInputReport(OSAction * action, IOReturn status, uint32_t actualByteCount, uint64_t completionTimestamp);
```

## Parameters 

`action`  

The completion action.

`status`  

The completion status.

`actualByteCount`  

The number of bytes read.

## Discussion

If an asynchronous request for an input report was successful, this method handles the report and schedules a new asynchronous request for an updated report. If the request was unsuccessful, this method retries the initial request, resetting the USB device as needed if it is unresponsive.

## See Also

### Managing Device Reports

newReportDescriptor

Returns the data in the HID device’s report descriptor.

getReport

Gets a report from the HID device.

getReport

Gets a report from the HID device.

setReport

Sends a report to the HID device.

initInputReport

Starts reading the input report from the device.

scheduleInputReportRetry

Retries a previous request for an input report.

cancelInputReportRetry

Cancels a retry attempt for an input report request.

TimerOccurred

Handles timeout-related actions when retrying input report requests.

