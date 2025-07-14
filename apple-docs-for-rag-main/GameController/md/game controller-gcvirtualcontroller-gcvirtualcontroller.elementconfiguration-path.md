

- Game Controller
- GCVirtualController
- GCVirtualController.ElementConfiguration
-  path 

Instance Property

# path

The Bezier path for the shape of an element.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
var path: UIBezierPath? { get set }
```

## Discussion

Use this property to customize the image of an element. The framework only supports custom paths for button elements.

## See Also

### Configuring elements

var isHidden: Bool

A Boolean value that determines whether the virtual controller hides the element.

var actsAsTouchpad: Bool

A Boolean value that determines whether the thumbstick element behaves as a touchpad.

