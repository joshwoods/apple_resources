

- HIDDriverKit
- IOUserHIDEventDriver
-  parsePointerElement 

Instance Method

# parsePointerElement

Parses an element to see if it supports pointer usages.

DriverKit 19.0+macOS

``` source
bool parsePointerElement(IOHIDElement * element);
```

## Parameters 

`element`  

An `IOHIDElement` object to parse.

## Return Value

`true` on success, otherwise `false`.

## Discussion

This method checks the element to determine if it contains pointer data suitable for dispatching in an event. If it does, the method stores a reference to the element for later use. When the driver object receives subsequent reports from the device, it uses the information in the stored pointer elements to dispatch pointer-specific events.

## See Also

### Parsing the Element Hierarchy

parseElements

Parses the specified array of elements.

parseDigitizerElement

Parses an element to see if it supports digitizer usages.

parseKeyboardElement

Parses an element to see if it contains keyboard-related information.

parseScrollElement

Parses an element to see if it supports scroll usages.

parseLEDElement

Parses an element to see if it supports LED usages.

