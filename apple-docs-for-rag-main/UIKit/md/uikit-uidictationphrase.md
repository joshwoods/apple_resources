

- UIKit
-  UIDictationPhrase 

Class

# UIDictationPhrase

An object that represents the textual interpretation of a spoken phrase that the user dictates.

iOS 5.1+iPadOS 5.1+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UIDictationPhrase
```

## Overview

When the user chooses dictation input on a supported device, the system automatically inserts recognized phrases into the current text view. You can use an object of the UIDictationPhrase class to obtain a string representing a phrase a user has dictated. In the case of ambiguous dictation results, a dictation phrase object provides an array containing alternative strings. Methods in the UITextInput protocol allow your app to respond to the completion of dictation.

## Topics

### Obtaining textual interpretations of spoken text

var alternativeInterpretations: [String]?

An array of alternative textual interpretations of a dictated phrase.

var text: String

The most likely textual interpretation of a dictated phrase.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
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

class UITextInputMode

The current text input mode.

class UITextInputAssistantItem

An object that manages custom bar button items that you add to the shortcuts bar above the keyboard on iPad.

