

- Game Controller
- GCPhysicalInputProfile
-  elements 

Instance Property

# elements

The elements in the profile as key-value pairs for lookup by name.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var elements: [String : GCControllerElement] { get }
```

## Discussion

Use this property to access elements by name. For example, use the name `“Button A”` to get the face button of an extended gamepad profile.

```
button = physicalInputProfile.elements[“Button A”]
```

For more button names, see Extended gamepad input names.

## See Also

### Accessing elements by name or key

var buttons: [String : GCControllerButtonInput]

The buttons in the profile as key-value pairs for lookup by name.

var axes: [String : GCControllerAxisInput]

The axes in the profile as key-value pairs for lookup by name.

var dpads: [String : GCControllerDirectionPad]

The directional pads in the profile as key-value pairs for lookup by name.

var touchpads: [String : GCControllerTouchpad]

The touchpads in the profile as key-value pairs for lookup by name.

subscript(String) -> GCControllerElement?

Returns the element that the key specifies.

