

- HIDDriverKit
- IOUserUSBHostHIDDevice
-  cancelInputReportRetry 

Instance Method

# cancelInputReportRetry

Cancels a retry attempt for an input report request.

DriverKit 19.0+macOS

``` source
void cancelInputReportRetry();
```

## Discussion

Don’t call this method directly. The CompleteInputReport method calls it automatically when a retry attempt succeeds.

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

scheduleInputReportRetry

Retries a previous request for an input report.

TimerOccurred

Handles timeout-related actions when retrying input report requests.

