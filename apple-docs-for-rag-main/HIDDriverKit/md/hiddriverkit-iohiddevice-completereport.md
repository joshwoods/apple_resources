

- HIDDriverKit
- IOHIDDevice
-  CompleteReport 

Instance Method

# CompleteReport

Completes all async requests made when getting or setting a report.

DriverKit 19.0+macOS

``` source
void CompleteReport(OSAction * action, IOReturn status, uint32_t actualByteCount);
```

## Parameters 

`action`  

The action passed to the `getReport` or `setReport` methods.

`status`  

The completion status.

`actualByteCount`  

The size of the buffer sent to the `getReport` or `setReport` methods.

## Discussion

Call this method upon completion of the getReport and setReport methods.

## See Also

### Processing Device Reports

handleReport

Handles an asynchronous report received from the HID device.

getReport

Gets a report from the HID device.

setReport

Sends a report to the HID device.

Report Options

The enumerated report options.

