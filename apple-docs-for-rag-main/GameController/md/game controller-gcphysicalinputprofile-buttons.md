

- Game Controller
- GCPhysicalInputProfile
-  buttons 

Instance Property

# buttons

The buttons in the profile as key-value pairs for lookup by name.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var buttons: [String : GCControllerButtonInput] { get }
```

## Discussion

Use the GCInputXboxPaddleOne constant to get the P1 paddle button for an Xbox controller.

```
button = physicalInputProfile.buttons[GCInputXboxPaddleOne]
```

For more button names, see Extended gamepad input names and Xbox controller input names.

## See Also

### Accessing elements by name or key

var elements: [String : GCControllerElement]

The elements in the profile as key-value pairs for lookup by name.

var axes: [String : GCControllerAxisInput]

The axes in the profile as key-value pairs for lookup by name.

var dpads: [String : GCControllerDirectionPad]

The directional pads in the profile as key-value pairs for lookup by name.

var touchpads: [String : GCControllerTouchpad]

The touchpads in the profile as key-value pairs for lookup by name.

subscript(String) -> GCControllerElement?

Returns the element that the key specifies.

