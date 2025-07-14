

- UIKit
- UITextInputTraits
-  returnKeyType 

Instance Property

# returnKeyType

The visible title of the Return key.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
optional var returnKeyType: UIReturnKeyType { get set }
```

## Discussion

Setting this property to a different key type changes the visible title of the Return key and typically results in the keyboard being dismissed when it is pressed. The default value for this property is UIReturnKeyType.default.

## See Also

### Configuring the keyboard appearance

var keyboardType: UIKeyboardType

The keyboard type for the text object.

enum UIKeyboardType

Constants that specify the type of keyboard to display for a text-based view.

var keyboardAppearance: UIKeyboardAppearance

The appearance style of the keyboard for the text object.

enum UIKeyboardAppearance

Constants that specify the appearance of the keyboard for a text-based view.

enum UIReturnKeyType

Constants that specify the text string that displays in the Return key of a keyboard.

var textContentType: UITextContentType!

The semantic meaning for a text input area.

struct UITextContentType

Constants that identify the semantic meaning for a text-entry area.

