

- UIKit
- UITextInputTraits
-  keyboardAppearance 

Instance Property

# keyboardAppearance

The appearance style of the keyboard for the text object.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
optional var keyboardAppearance: UIKeyboardAppearance { get set }
```

## Discussion

This property lets you distinguish between the default text entry inside your application and text entry inside an alert panel. The default value for this property is UIKeyboardAppearance.default.

## See Also

### Configuring the keyboard appearance

var keyboardType: UIKeyboardType

The keyboard type for the text object.

enum UIKeyboardType

Constants that specify the type of keyboard to display for a text-based view.

enum UIKeyboardAppearance

Constants that specify the appearance of the keyboard for a text-based view.

var returnKeyType: UIReturnKeyType

The visible title of the Return key.

enum UIReturnKeyType

Constants that specify the text string that displays in the Return key of a keyboard.

var textContentType: UITextContentType!

The semantic meaning for a text input area.

struct UITextContentType

Constants that identify the semantic meaning for a text-entry area.

