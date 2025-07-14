

- HIDDriverKit
- IOHIDDevice
-  Report Options 

API Collection

# Report Options

The enumerated report options.

## Topics

### Getting the Report Options

kIOHIDReportOptionNotInterrupt

An option that indicates the report isn’t interrupt driven.

kIOHIDReportOptionVariableSize

An option that indicates the report has a variable size.

## See Also

### Processing Device Reports

handleReport

Handles an asynchronous report received from the HID device.

getReport

Gets a report from the HID device.

setReport

Sends a report to the HID device.

CompleteReport

Completes all async requests made when getting or setting a report.

