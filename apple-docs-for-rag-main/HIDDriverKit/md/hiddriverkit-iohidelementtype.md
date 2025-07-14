

- HIDDriverKit
-  IOHIDElementType 

Enumeration

# IOHIDElementType

The types of HID elements that you can examine.

DriverKitmacOS

``` source
enum IOHIDElementType : unsigned int;
```

## Overview

Use this type to identify the type of an element you are using. The type is also the value for the key `kIOHIDElementTypeKey` in the dictionary describing the element.

## Topics

### Getting the Element Types

kIOHIDElementTypeInput_Misc

The element contains an input data field of varying size.

kIOHIDElementTypeInput_Button

The element contains a one-bit input data field.

kIOHIDElementTypeInput_Axis

The element contains an axis of movement.

kIOHIDElementTypeInput_ScanCodes

The element contains an input field with a scan code or usage selector.

kIOHIDElementTypeInput_NULL

The element signals the end of an input data field in an input report.

kIOHIDElementTypeOutput

The element contains a data field in an output report.

kIOHIDElementTypeFeature

The element contains input and output data not intended for consumption by the end user.

kIOHIDElementTypeCollection

The element acts as a parent container for two or more related elements.

## See Also

### Managing the Element Hierarchy

getType

getCollectionType

getChildElements

getParentElement

IOHIDElementCollectionType

Constants that indicate the types of relationships that exist between two or more elements.

