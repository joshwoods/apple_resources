

- WatchKit
- WKInterfaceObject
-  interfaceProperty 

Instance Property

# interfaceProperty

The name of the outlet in your interface controller to which the object is bound.

watchOS 2.0+

``` source
var interfaceProperty: String { get }
```

## Discussion

The string in this property corresponds to the name of a property in one of your WKInterfaceController subclasses. WatchKit uses this value internally to manage the connection between the interface object and the corresponding object on Apple Watch. You do not need to use this property directly.

