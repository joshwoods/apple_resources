

- HIDDriverKit
-  IOHIDElementCollectionType 

Enumeration

# IOHIDElementCollectionType

Constants that indicate the types of relationships that exist between two or more elements.

DriverKitmacOS

``` source
enum IOHIDElementCollectionType : unsigned int;
```

## Topics

### Getting the Element Collection Types

kIOHIDElementCollectionTypePhysical

A collection in which the child elements are data points collected at one geometric point.

kIOHIDElementCollectionTypeApplication

A collection in which the child elements serve different purposes in a single device.

kIOHIDElementCollectionTypeLogical

A collection in which the child elements form a composite data structure.

kIOHIDElementCollectionTypeReport

A collection that wraps all the other elements in a report.

kIOHIDElementCollectionTypeNamedArray

A collection in which the elements are an array of selector usages.

kIOHIDElementCollectionTypeUsageSwitch

A collection that modifies the meaning of the usage it contains.

kIOHIDElementCollectionTypeUsageModifier

A collection that modifies the meaning of the usage attached to the encompassing collection.

## See Also

### Managing the Element Hierarchy

getType

getCollectionType

getChildElements

getParentElement

IOHIDElementType

The types of HID elements that you can examine.

