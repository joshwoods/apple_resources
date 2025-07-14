

- HIDDriverKit
- IOHIDDevice
-  handleReport 

Instance Method

# handleReport

Handles an asynchronous report received from the HID device.

DriverKit 19.0+macOS

``` source
kern_return_t handleReport(uint64_t timestamp, IOMemoryDescriptor * report, uint32_t reportLength, IOHIDReportType reportType, IOOptionBits options);
```

## Parameters 

`report`  

A memory descriptor that describes the report.

`reportType`  

The type of report.

`options`  

Options to specify in the request. No options are currently supported, and the default value is `0`.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

The default implementation of this method parses the report data and notifies attached interfaces of any changes.

## See Also

### Processing Device Reports

getReport

Gets a report from the HID device.

setReport

Sends a report to the HID device.

CompleteReport

Completes all async requests made when getting or setting a report.

Report Options

The enumerated report options.

