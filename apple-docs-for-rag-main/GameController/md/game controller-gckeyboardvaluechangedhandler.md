

- Game Controller
-  GCKeyboardValueChangedHandler 

Type Alias

# GCKeyboardValueChangedHandler

The signature for the block that the keyboard input profile calls when a key value changes.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
typealias GCKeyboardValueChangedHandler = (GCKeyboardInput, GCControllerButtonInput, GCKeyCode, Bool) -> Void
```

## Parameters 

`keyboard`  

The keyboard controller profile for the physical keyboard.

`key`  

The element for the key that changes.

`keyCode`  

The code for the key that changes.

`pressed`  

true if the user presses the key at the time the change occurs; otherwise, false.

## See Also

### Getting Change Information

var keyChangedHandler: GCKeyboardValueChangedHandler?

The block that the profile calls when the user presses a key.

