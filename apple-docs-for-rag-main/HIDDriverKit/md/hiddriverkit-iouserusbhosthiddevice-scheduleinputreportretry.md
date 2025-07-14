

- HIDDriverKit
- IOUserUSBHostHIDDevice
-  scheduleInputReportRetry 

Instance Method

# scheduleInputReportRetry

Retries a previous request for an input report.

DriverKit 19.0+macOS

``` source
void scheduleInputReportRetry(kern_return_t reason);
```

## Parameters 

`reason`  

The reason the previous request failed.

## Discussion

Don’t call this method directly. The CompleteInputReport method calls it automatically to retry the previous request for the input report.

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

CompleteInputReport

Processes the results of an asynchronous request for an input report.

cancelInputReportRetry

Cancels a retry attempt for an input report request.

TimerOccurred

Handles timeout-related actions when retrying input report requests.

