

- HIDDriverKit
- IOUserHIDEventService
-  getElements 

Instance Method

# getElements

Returns an array of elements that contain the parsed data from the HID device’s report.

DriverKit 19.0+macOS

``` source
OSArray * getElements();
```

## Return Value

An array of IOHIDElement objects containing the parsed data from the report.

## Discussion

Use this method to get the array of IOHIDElement objects that contain the data for the most recent device report. Each element contains data for a single aspect of the device’s state. For example, a report from a stylus contains separate elements for the horizontal and vertical position of the stylus, the pressure values, and so on. Use the getUsagePage and getUsage methods of the element to determine the type of information in each element.

This method creates a new set of IOHIDElement objects the first time you call it. On subequent calls, it updates the existing IOHIDElement objects with data from the most recent report.

## See Also

### Responding to Input Reports

handleReport

Converts an incoming device report into dispatchable events.

ReportAvailable

Notifies the event service that an updated report is available from the HID device.

