

- Game Controller
- GCPhysicalInputProfile
-  touchpads 

Instance Property

# touchpads

The touchpads in the profile as key-value pairs for lookup by name.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var touchpads: [String : GCControllerTouchpad] { get }
```

## See Also

### Accessing elements by name or key

var elements: [String : GCControllerElement]

The elements in the profile as key-value pairs for lookup by name.

var buttons: [String : GCControllerButtonInput]

The buttons in the profile as key-value pairs for lookup by name.

var axes: [String : GCControllerAxisInput]

The axes in the profile as key-value pairs for lookup by name.

var dpads: [String : GCControllerDirectionPad]

The directional pads in the profile as key-value pairs for lookup by name.

subscript(String) -> GCControllerElement?

Returns the element that the key specifies.

