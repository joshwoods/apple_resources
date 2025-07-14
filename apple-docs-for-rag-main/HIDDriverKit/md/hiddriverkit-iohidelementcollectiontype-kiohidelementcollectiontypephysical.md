

- HIDDriverKit
- IOHIDElementCollectionType
-  kIOHIDElementCollectionTypePhysical 

Enumeration Case

# kIOHIDElementCollectionTypePhysical

A collection in which the child elements are data points collected at one geometric point.

DriverKitmacOS

``` source
kIOHIDElementCollectionTypePhysical
```

## Discussion

A sensing device might associate sets of measured or sensed data with a single point. This type does not indicate that multiple data values come from the device.

## See Also

### Getting the Element Collection Types

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

