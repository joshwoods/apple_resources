

- HIDDriverKit
- IOUserUSBHostHIDDevice
-  TimerOccurred 

Instance Method

# TimerOccurred

Handles timeout-related actions when retrying input report requests.

DriverKit 19.0+macOS

``` source
void TimerOccurred(OSAction * action, uint64_t time);
```

## Parameters 

`action`  

The timer action.

`time`  

The time.

## Discussion

Don’t call this method directly. When the service needs to retry an input request, it delays the start of that request by a short amount of time. This method processes that delay and begins the new request.

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

cancelInputReportRetry

Cancels a retry attempt for an input report request.

