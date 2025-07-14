

- Game Controller
- GCVirtualController
- GCVirtualController.Configuration
-  isHidden 

Instance Property

# isHidden

A Boolean value that indicates whether the system or the app presents the virtual interface.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
var isHidden: Bool { get set }
```

## Discussion

To present your own virtual controller interface, set this property to true. Then when the state of controls in your interface changes, use the GCVirtualController setValue(_:forButtonElement:) and setPosition(_:forDirectionPadElement:) methods to update the corresponding elements.

The default value is false.

