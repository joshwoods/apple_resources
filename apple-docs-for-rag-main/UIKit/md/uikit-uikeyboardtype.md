

- UIKit
-  UIKeyboardType 

Enumeration

# UIKeyboardType

Constants that specify the type of keyboard to display for a text-based view.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
enum UIKeyboardType
```

## Overview

Use these constants with the keyboardType property.

## Topics

### Constants

case `default`

Specifies the default keyboard for the current input method.

case asciiCapable

Specifies a keyboard that displays standard ASCII characters.

case numbersAndPunctuation

Specifies the numbers and punctuation keyboard.

case URL

Specifies a keyboard for URL entry.

case numberPad

Specifies a numeric keypad for PIN entry.

case phonePad

Specifies a keypad for entering telephone numbers.

case namePhonePad

Specifies a keypad for entering a person’s name or phone number.

case emailAddress

Specifies a keyboard for entering email addresses.

case decimalPad

Specifies a keyboard with numbers and a decimal point.

case twitter

Specifies a keyboard for Twitter text entry, with easy access to the at (”`@`”) and hash (”`#`”) characters.

case webSearch

Specifies a keyboard for web search terms and URL entry.

case asciiCapableNumberPad

Specifies a number pad that outputs only ASCII digits.

static var alphabet: UIKeyboardType

Specifies a keyboard for alphabetic entry.

Deprecated

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring the keyboard appearance

var keyboardType: UIKeyboardType

The keyboard type for the text object.

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

