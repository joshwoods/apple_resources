

- Kernel
- Hardware Families
- HID
-  IOHIDElementType 

Type Alias

# IOHIDElementType

Describes different types of HID elements.

macOS 10.0+

``` source
typedef enum IOHIDElementType IOHIDElementType;
```

## Discussion

Used by the IOHIDFamily to identify the type of element processed. Represented by the key kIOHIDElementTypeKey in the dictionary describing the element.

## Topics

### Constants

kIOHIDElementTypeInput_Misc

kIOHIDElementTypeInput_Button

kIOHIDElementTypeInput_Axis

kIOHIDElementTypeInput_ScanCodes

kIOHIDElementTypeOutput

kIOHIDElementTypeFeature

kIOHIDElementTypeCollection

kIOHIDElementTypeInput_NULL

## See Also

### HID Elements

IOHIDElementCollectionType

Describes different types of HID collections.

IOHIDElementCommitDirection

IOHIDElementCookie

Abstract data type used as a unique identifier for an element.

IOHIDElementFlags

IOHIDValueOptions

Describes options for gathering element values.

### Related Documentation

IOHIDElementType

Describes different types of HID elements.

