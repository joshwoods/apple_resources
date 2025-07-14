

- Game Controller
- GCPhysicalInputProfile
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Returns the element that the key specifies.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
subscript(key: String) -> GCControllerElement? { get }
```

## Parameters 

`key`  

A key that identifies an element.

## Return Value

The element that matches the key.

## Discussion

You can access elements of a profile using a subscript notation. For example, get the button with the X label from an instance of GCMicroGamepad using `microGamepad[”Button X”]`.

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

var touchpads: [String : GCControllerTouchpad]

The touchpads in the profile as key-value pairs for lookup by name.

