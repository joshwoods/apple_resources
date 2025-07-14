

- UIKit
- UITextInputTraits
-  keyboardType 

Instance Property

# keyboardType

The keyboard type for the text object.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
optional var keyboardType: UIKeyboardType { get set }
```

## Mentioned in 

Configuring a custom keyboard interface

## Discussion

Text objects can be targeted for specific types of input, such as plain text, email, numeric entry, and so on. The keyboard style identifies what keys are available on the keyboard and which ones appear by default. The default value for this property is UIKeyboardType.default.

## See Also

### Configuring the keyboard appearance

enum UIKeyboardType

Constants that specify the type of keyboard to display for a text-based view.

var keyboardAppearance: UIKeyboardAppearance

The appearance style of the keyboard for the text object.

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

