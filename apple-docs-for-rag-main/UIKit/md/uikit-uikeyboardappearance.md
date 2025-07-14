

- UIKit
-  UIKeyboardAppearance 

Enumeration

# UIKeyboardAppearance

Constants that specify the appearance of the keyboard for a text-based view.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
enum UIKeyboardAppearance
```

## Overview

Use these constants with the keyboardAppearance property.

## Topics

### Constants

case `default`

Specifies the default keyboard appearance for the current input method.

case dark

Specifies a keyboard appearance suitable for a dark UI look.

case light

Specifies a keyboard appearance suitable for a light UI look.

static var alert: UIKeyboardAppearance

Specifies a keyboard appearance suitable for an alert panel.

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

enum UIKeyboardType

Constants that specify the type of keyboard to display for a text-based view.

var keyboardAppearance: UIKeyboardAppearance

The appearance style of the keyboard for the text object.

var returnKeyType: UIReturnKeyType

The visible title of the Return key.

enum UIReturnKeyType

Constants that specify the text string that displays in the Return key of a keyboard.

var textContentType: UITextContentType!

The semantic meaning for a text input area.

struct UITextContentType

Constants that identify the semantic meaning for a text-entry area.

