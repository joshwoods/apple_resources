

- HIDDriverKit
- IOUserHIDEventDriver
-  parseDigitizerElement 

Instance Method

# parseDigitizerElement

Parses an element to see if it supports digitizer usages.

DriverKit 19.0+macOS

``` source
bool parseDigitizerElement(IOHIDElement * element);
```

## Parameters 

`element`  

An `IOHIDElement` object to parse.

## Return Value

`true` on success, otherwise `false`.

## Discussion

This method checks the element to determine if it contains digitizer data suitable for dispatching in an event. If it does, the method stores a reference to the element for later use. When the driver object receives subsequent reports from the device, it uses the information in the stored digitizer elements to dispatch digitizer-specific events.

## See Also

### Parsing the Element Hierarchy

parseElements

Parses the specified array of elements.

parsePointerElement

Parses an element to see if it supports pointer usages.

parseKeyboardElement

Parses an element to see if it contains keyboard-related information.

parseScrollElement

Parses an element to see if it supports scroll usages.

parseLEDElement

Parses an element to see if it supports LED usages.

