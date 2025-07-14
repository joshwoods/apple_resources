

- UIKit
-  UIReturnKeyType 

Enumeration

# UIReturnKeyType

Constants that specify the text string that displays in the Return key of a keyboard.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
enum UIReturnKeyType
```

## Overview

Use these constants with the returnKeyType property.

## Topics

### Constants

case `default`

Specifies that the visible title of the Return key is *return*.

case go

Specifies that the visible title of the Return key is *Go*.

case google

Specifies that the visible title of the Return key is *Google*.

case join

Specifies that the visible title of the Return key is *Join*.

case next

Specifies that the visible title of the Return key is *Next*.

case route

Specifies that the visible title of the Return key is *Route*.

case search

Specifies that the visible title of the Return key is *Search*.

case send

Specifies that the visible title of the Return key is *Send*.

case yahoo

Specifies that the visible title of the Return key is *Yahoo*.

case done

Specifies that the visible title of the Return key is *Done*.

case emergencyCall

Specifies that the visible title of the Return key is *Emergency Call*.

case `continue`

Specifies that the visible title of the Return key is *Continue*.

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

enum UIKeyboardAppearance

Constants that specify the appearance of the keyboard for a text-based view.

var returnKeyType: UIReturnKeyType

The visible title of the Return key.

var textContentType: UITextContentType!

The semantic meaning for a text input area.

struct UITextContentType

Constants that identify the semantic meaning for a text-entry area.

