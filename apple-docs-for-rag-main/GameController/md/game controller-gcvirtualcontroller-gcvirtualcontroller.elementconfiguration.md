

- Game Controller
- GCVirtualController
-  GCVirtualController.ElementConfiguration 

Class

# GCVirtualController.ElementConfiguration

The properties of a virtual controller’s element that you can customize.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
class ElementConfiguration
```

## Topics

### Configuring elements

var path: UIBezierPath?

The Bezier path for the shape of an element.

var isHidden: Bool

A Boolean value that determines whether the virtual controller hides the element.

var actsAsTouchpad: Bool

A Boolean value that determines whether the thumbstick element behaves as a touchpad.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Customizing the elements

func updateConfiguration(forElement: String, configuration: (GCVirtualController.ElementConfiguration) -> GCVirtualController.ElementConfiguration)

Changes the configuration for one of the virtual controller’s input elements.

