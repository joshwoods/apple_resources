

- HIDDriverKit
- IOUserHIDEventDriver
-  handleReport 

Instance Method

# handleReport

Processes the information in a new device report and dispatches any relevant events in response.

DriverKit 19.0+macOS

``` source
void handleReport(uint64_t timestamp, uint8_t * report, uint32_t reportLength, IOHIDReportType type, uint32_t reportID);
```

## Parameters 

`timestamp`  

The timestamp of the report.

`report`  

A pointer to the raw bytes of the report.

`reportLength`  

The number of bytes of data in the `report` parameter.

`type`  

The report type.

`reportID`  

The unique ID associated with the report. If a report element has new data, it contains this ID.

## Discussion

This method iterates over the elements in the report and dispatches events for any changed values. The system calls this method automatically when a new report arrives; don’t call this method yourself.

## See Also

### Handling New Data Reports

handleKeyboardReport

Iterates through keyboard elements and dispatches them if the element value has been updated.

handleRelativePointerReport

Iterates through relative pointer elements and dispatches them if the element value has been updated.

handleAbsolutePointerReport

Iterates through absolute pointer elements and dispatches them if the element value has been updated.

handleScrollReport

Iterates through scroll elements and dispatches them if the element value has been updated.

handleDigitizerReport

Processes the digitizer elements and dispatches events for any updated values.

createEventForDigitizerCollection

Creates a HID event object that represents a digitizer collection.

