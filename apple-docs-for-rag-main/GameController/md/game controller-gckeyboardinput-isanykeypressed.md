

- Game Controller
- GCKeyboardInput
-  isAnyKeyPressed 

Instance Property

# isAnyKeyPressed

A Boolean value that indicates whether the user is pressing any of the keys.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var isAnyKeyPressed: Bool { get }
```

## Discussion

If true, the user is pressing a key; otherwise, the user isn’t. You can use this property to check whether the user presses any key before getting the state of specific keys.

## See Also

### Accessing Buttons

func button(forKeyCode: GCKeyCode) -> GCControllerButtonInput?

Returns the button element for the specified key code.

struct GCKeyCode

The key codes for keys on a keyboard.

Keycode Constants

Constants for the codes of keyboard keys.

