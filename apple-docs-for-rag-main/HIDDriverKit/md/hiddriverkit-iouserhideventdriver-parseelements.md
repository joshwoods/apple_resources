

- HIDDriverKit
- IOUserHIDEventDriver
-  parseElements 

Instance Method

# parseElements

Parses the specified array of elements.

DriverKit 19.0+macOS

``` source
bool parseElements(OSArray * elements);
```

## Parameters 

`elements`  

An array of IOHIDElement objects to parse.

## Return Value

`true` if parsing was successful, or `false` if an error occurred.

## Discussion

This method searches the elements array for IOHIDElement objects relevant to keyboard, digitizer, pointer, scrolling, and LED events. It stores a reference to each relevant element it finds, and uses those objects later to obtain relevant information for events.

The driver’s Start method calls this method, so you don’t need to call it directly.

## See Also

### Parsing the Element Hierarchy

parsePointerElement

Parses an element to see if it supports pointer usages.

parseDigitizerElement

Parses an element to see if it supports digitizer usages.

parseKeyboardElement

Parses an element to see if it contains keyboard-related information.

parseScrollElement

Parses an element to see if it supports scroll usages.

parseLEDElement

Parses an element to see if it supports LED usages.

