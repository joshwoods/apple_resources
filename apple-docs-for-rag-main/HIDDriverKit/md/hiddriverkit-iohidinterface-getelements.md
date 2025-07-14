

- HIDDriverKit
- IOHIDInterface
-  getElements 

Instance Method

# getElements

Returns the array of elements that the interface uses to store parsed report data.

DriverKit 19.0+macOS

``` source
OSArray * getElements();
```

## Return Value

An array of IOHIDElement objects containing the parsed data from the report.

## Discussion

This method returns the array of IOHIDElement objects associated with the interface. Each element contains data for a single aspect of the device’s state. For example, a report from a stylus contains separate elements for the horizontal and vertical position of the stylus, the pressure values, and so on. Use the getUsagePage and getUsage methods of the element to determine the type of information in each element.

This method creates a new set of `IOHIDElement` objects the first time you call it, but it doesn’t update the contents of each element automatically. Call the processReport method to update the contents of the elements before using this method to retrieve them.

## See Also

### Accessing the Elements of a Report

commitElements

Gets or sets the contents of the interface’s stored elements.

