

- Game Controller
- GCKeyboardInput
-  keyChangedHandler 

Instance Property

# keyChangedHandler

The block that the profile calls when the user presses a key.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var keyChangedHandler: GCKeyboardValueChangedHandler? { get set }
```

## Discussion

If multiple keys change values at the same time, the profile calls this block once for each key that changes.

## See Also

### Getting Change Information

typealias GCKeyboardValueChangedHandler

The signature for the block that the keyboard input profile calls when a key value changes.

