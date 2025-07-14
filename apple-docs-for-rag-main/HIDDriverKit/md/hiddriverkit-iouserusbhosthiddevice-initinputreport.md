

- HIDDriverKit
- IOUserUSBHostHIDDevice
-  initInputReport 

Instance Method

# initInputReport

Starts reading the input report from the device.

DriverKit 19.0+macOS

``` source
kern_return_t initInputReport();
```

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

This method requests the input report from the USB device asynchronously, delivering the results to the CompleteInputReport method.

You don’t need to call this method directly. The service’s Start method calls it when the service first runs, and the service requests new input reports regularly.

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

CompleteInputReport

Processes the results of an asynchronous request for an input report.

scheduleInputReportRetry

Retries a previous request for an input report.

cancelInputReportRetry

Cancels a retry attempt for an input report request.

TimerOccurred

Handles timeout-related actions when retrying input report requests.

