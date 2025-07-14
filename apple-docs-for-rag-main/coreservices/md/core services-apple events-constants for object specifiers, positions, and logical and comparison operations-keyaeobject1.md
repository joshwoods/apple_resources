

- Core Services
- Apple Events
- Constants for Object Specifiers, Positions, and Logical and Comparison Operations
-  keyAEObject1 

Global Variable

# keyAEObject1

Mac Catalyst 13.0+macOS 10.0+

``` source
var keyAEObject1: Int { get }
```

## Discussion

Identifies a descriptor for the element that is currently being compared to the object or data specified by the descriptor for the keyword `keyAEObject2`. Either object can be described by a descriptor of type `typeObjectSpecifier` or `typeObjectBeingExamined`.

A descriptor of `typeObjectBeingExamined` acts as a placeholder for each of the successive elements in a container when the Apple Event Manager tests those elements one at a time.

