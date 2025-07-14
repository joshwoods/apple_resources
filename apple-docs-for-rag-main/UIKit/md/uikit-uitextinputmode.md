

- UIKit
-  UITextInputMode 

Class

# UITextInputMode

The current text input mode.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UITextInputMode
```

## Overview

You can use this object to determine the primary language currently being used for text input.

## Topics

### Getting the current and active text-input modes

class var activeInputModes: [UITextInputMode]

The active text-input modes.

### Getting the primary language

var primaryLanguage: String?

The primary language, if any, of the input mode.

### Notifications

class let currentInputModeDidChangeNotification: NSNotification.Name

A notification that posts when the current input mode changes.

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
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Text input

protocol UITextInput

A set of methods for interacting with the text input system and enabling features in documents.

protocol UITextInputDelegate

An intermediary between a document and the text input system.

protocol UIKeyInput

A set of methods a responder uses to implement simple text entry.

protocol UITextInputTraits

A set of methods that defines features for keyboard input to a text object.

class UITextInputContext

An object that reports the type of input your app receives.

class UITextInputAssistantItem

An object that manages custom bar button items that you add to the shortcuts bar above the keyboard on iPad.

class UIDictationPhrase

An object that represents the textual interpretation of a spoken phrase that the user dictates.

