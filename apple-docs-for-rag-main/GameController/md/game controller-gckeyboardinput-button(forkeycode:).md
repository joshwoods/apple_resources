

- Game Controller
- GCKeyboardInput
-  button(forKeyCode:) 

Instance Method

# button(forKeyCode:)

Returns the button element for the specified key code.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func button(forKeyCode code: GCKeyCode) -> GCControllerButtonInput?
```

## Parameters 

`code`  

The code for the keyboard button element.

## Return Value

The keyboard button element that this profile defines for the specified key code.

## Discussion

Alternatively, you can get a button element for a key using the subscript(_:) notation that you inherit from GCPhysicalInputProfile, as in `keyboard[GCKeyUpArrow]`.

## See Also

### Accessing Buttons

var isAnyKeyPressed: Bool

A Boolean value that indicates whether the user is pressing any of the keys.

struct GCKeyCode

The key codes for keys on a keyboard.

Keycode Constants

Constants for the codes of keyboard keys.

