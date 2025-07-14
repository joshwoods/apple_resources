

- UIKit
-  UIKey 

Class

# UIKey

An object that provides information about the state of a keyboard key.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+tvOS 13.4+visionOS 1.0+

``` source
@MainActor
class UIKey
```

## Overview

UIKey provides relevant information about the current state of a key on a keyboard as a user presses and releases the key. To learn more, see Handling key presses made on a physical keyboard.

## Topics

### Determining key type

var keyCode: UIKeyboardHIDUsage

The HID usage code of the key.

var modifierFlags: UIKeyModifierFlags

The modifier keys pressed and held while the user presses the key.

### Getting key characters

var characters: String

A string that represents the text value of the key combined with any active modifier keys.

var charactersIgnoringModifiers: String

A string that represents the text value of the key without modifier keys.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- Sendable

## See Also

### Physical keyboards

Handling key presses made on a physical keyboard

Detect when someone presses and releases keys on a physical keyboard.

Navigating an app’s user interface using a keyboard

Navigate between user interface elements using a keyboard and focusable UI elements in iPad apps and apps built with Mac Catalyst.

Adding hardware keyboard support to your app

Enhance interactions with your app by handling raw keyboard events, writing custom keyboard shortcuts, and working with gesture recognizers.

enum UIKeyboardHIDUsage

A set of HID usage codes that identify the keys of a USB keyboard.

