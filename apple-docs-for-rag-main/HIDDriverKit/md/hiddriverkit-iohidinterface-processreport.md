

- HIDDriverKit
- IOHIDInterface
-  processReport 

Instance Method

# processReport

Parses the contents of the specified report and updates the interface’s elements.

DriverKit 19.0+macOS

``` source
void processReport(uint64_t timestamp, uint8_t * report, uint32_t reportLength, IOHIDReportType type, uint32_t reportID);
```

## Parameters 

`timestamp`  

The timestamp of the report.

`report`  

A pointer to the bytes of the report.

`reportLength`  

The number of bytes in the `report` parameter.

`type`  

The report type.

`reportID`  

The unique ID associated with the report.

## Discussion

This method uses the provided report data to update the IOHIDElement objects associated with this interface. Upon receiving a new report, call this method before you call the getElements method.

## See Also

### Getting and Setting Input Reports

ReportAvailable

Notifies the interface that an updated report is available from the HID device.

AddReportToPool

Adds a memory descriptor to the report pool.

GetReport

Retrieves a new input report from the HID device.

SetReport

Sends a report to the HID device.

