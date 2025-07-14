

- HIDDriverKit
- IOUserHIDEventDriver
-  handleDigitizerReport 

Instance Method

# handleDigitizerReport

Processes the digitizer elements and dispatches events for any updated values.

DriverKit 19.0+macOS

``` source
void handleDigitizerReport(uint64_t timestamp, uint32_t reportID);
```

## Parameters 

`timestamp`  

The timestamp of the input report.

`reportID`  

The report ID.

## Discussion

This method iterates over the digitizer elements from the report and dispatches events for any changed values. The system calls this method automatically when a new report arrives; don’t call this method yourself.

## See Also

### Handling New Data Reports

handleReport

Processes the information in a new device report and dispatches any relevant events in response.

handleKeyboardReport

Iterates through keyboard elements and dispatches them if the element value has been updated.

handleRelativePointerReport

Iterates through relative pointer elements and dispatches them if the element value has been updated.

handleAbsolutePointerReport

Iterates through absolute pointer elements and dispatches them if the element value has been updated.

handleScrollReport

Iterates through scroll elements and dispatches them if the element value has been updated.

createEventForDigitizerCollection

Creates a HID event object that represents a digitizer collection.

