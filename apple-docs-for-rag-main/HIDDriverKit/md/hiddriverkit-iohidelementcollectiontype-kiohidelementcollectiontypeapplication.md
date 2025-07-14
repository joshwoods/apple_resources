

- HIDDriverKit
- IOHIDElementCollectionType
-  kIOHIDElementCollectionTypeApplication 

Enumeration Case

# kIOHIDElementCollectionTypeApplication

A collection in which the child elements serve different purposes in a single device.

DriverKitmacOS

``` source
kIOHIDElementCollectionTypeApplication
```

## Discussion

A keyboard that contains an integrated pointing device might define separate application collections for the keyboard and pointing data.

## See Also

### Getting the Element Collection Types

kIOHIDElementCollectionTypePhysical

A collection in which the child elements are data points collected at one geometric point.

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

