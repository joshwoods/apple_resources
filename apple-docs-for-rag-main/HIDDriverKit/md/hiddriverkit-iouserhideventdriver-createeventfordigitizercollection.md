

- HIDDriverKit
- IOUserHIDEventDriver
-  createEventForDigitizerCollection 

Instance Method

# createEventForDigitizerCollection

Creates a HID event object that represents a digitizer collection.

DriverKit 19.0+macOS

``` source
IOHIDEvent * createEventForDigitizerCollection(IOHIDDigitizerCollection * collection, uint64_t timestamp, uint32_t reportID);
```

## Parameters 

`collection`  

A collection of IOHIDElement objects, each of which contains digitizer information to include in the event object.

`timestamp`  

The timestamp of the input report.

`reportID`  

The report ID.

## Return Value

An `IOHIDEvent` object containing the digitizer-related data. This method returns `NULL` if it encounters an error or if no elements in the collection contain updated values.

## Discussion

This method creates an `IOHIDEvent` object with any updated digitizer values that it finds. The handleDigitizerReport calls this method when processing an input report; don’t call this method directly.

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

handleDigitizerReport

Processes the digitizer elements and dispatches events for any updated values.

