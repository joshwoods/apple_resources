

- HIDDriverKit
- IOUserHIDEventService
-  ReportAvailable 

Instance Method

# ReportAvailable

Notifies the event service that an updated report is available from the HID device.

DriverKit 19.0+macOS

``` source
void ReportAvailable(uint64_t timestamp, uint32_t reportID, uint32_t reportLength, IOHIDReportType type, IOMemoryDescriptor * report, OSAction * action);
```

## Parameters 

`timestamp`  

The timestamp of the report.

`reportID`  

The unique ID associated with the report.

`reportLength`  

The length of the report in bytes.

`type`  

The report type.

`report`  

A memory descriptor that contains the raw data for the report.

`action`  

The `OSAction` object that handles the asynchronous report callback.

## Discussion

Implement a custom version of this method in your event service. Use the TYPE macro to let the system know that your method conforms to this prototype.

The system calls this method to notify your event service when a new report arrives.

## See Also

### Responding to Input Reports

getElements

Returns an array of elements that contain the parsed data from the HID device’s report.

handleReport

Converts an incoming device report into dispatchable events.

