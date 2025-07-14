

- UIKit
- UIKey
-  keyCode 

Instance Property

# keyCode

The HID usage code of the key.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+tvOS 13.4+visionOS 1.0+

``` source
@MainActor
var keyCode: UIKeyboardHIDUsage { get }
```

## Discussion

Use this property to determine the HID (Human Interface Device) usage code that identifies the key of a USB (Universal Serial Bus) keyboard. For a list of HID usage codes, see UIKeyboardHIDUsage.

Due to the variation of keyboards from language to language, it isn’t feasible to specify exact key mappings for every language. Where the HID usage code list isn’t specific for a key in a particular language, the keyboard firmware uses the closest equivalent key position so manufacturers can produce keyboards for different languages by simply printing different keycaps.

One example is the Y key on a North American keyboard. In Germany, the Z key typically occupies the Y key position. Rather than changing the keyboard firmware to put the Z usage code into that place in the descriptor list, the vendor uses the Y usage code on both the North American and German keyboards.

Because the key mapping may not be exact, use charactersIgnoringModifiers instead of keyCode to determine the text value of the key.

## See Also

### Determining key type

var modifierFlags: UIKeyModifierFlags

The modifier keys pressed and held while the user presses the key.

