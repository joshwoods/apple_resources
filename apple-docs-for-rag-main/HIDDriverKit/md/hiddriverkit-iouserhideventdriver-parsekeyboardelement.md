

- HIDDriverKit
- IOUserHIDEventDriver
-  parseKeyboardElement 

Instance Method

# parseKeyboardElement

Parses an element to see if it contains keyboard-related information.

DriverKit 19.0+macOS

``` source
bool parseKeyboardElement(IOHIDElement * element);
```

## Parameters 

`element`  

An `IOHIDElement` object to check.

## Return Value

`true` if the element contains relevant keyboard information, or `false` if it doesn’t.

## Discussion

This method checks the element to determine if it contains keyboard data suitable for dispatching in an event. If it does, the method stores a reference to the element for later use. When the driver object receives subsequent reports from the device, it uses the information in the stored keyboard elements to dispatch keyboard-specific events.

## See Also

### Parsing the Element Hierarchy

parseElements

Parses the specified array of elements.

parsePointerElement

Parses an element to see if it supports pointer usages.

parseDigitizerElement

Parses an element to see if it supports digitizer usages.

parseScrollElement

Parses an element to see if it supports scroll usages.

parseLEDElement

Parses an element to see if it supports LED usages.

