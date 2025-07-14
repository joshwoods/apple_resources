

- UIKit
-  UITextInputDelegate 

Protocol

# UITextInputDelegate

An intermediary between a document and the text input system.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
protocol UITextInputDelegate : NSObjectProtocol
```

## Mentioned in 

Handling text interactions in custom keyboards

## Overview

A UITextInputDelegate conveys notifications of pending or transpired changes in text and selection in the document. UIKit provides a private text input delegate, which it assigns at runtime to the inputDelegate property of the object whose class adopts the UITextInput protocol.

## Topics

### Notifying the delegate of textual changes

func textWillChange((any UITextInput)?)

Tells the input delegate when text is about to change in the document.

**Required**

func textDidChange((any UITextInput)?)

Tells the input delegate when text has changed in the document.

**Required**

### Notifying the delegate of selection changes

func selectionWillChange((any UITextInput)?)

Tells the input delegate when the selection is about to change in the document.

**Required**

func selectionDidChange((any UITextInput)?)

Tells the input delegate when the selection has changed in the document.

**Required**

### Notifying the delegate of conversation changes

func conversationContext(UIConversationContext?, didChange: (any UITextInput)?)

Tells the input delegate when text has changed in the input object for a conversation.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- UIInputViewController

## See Also

### Text input

protocol UITextInput

A set of methods for interacting with the text input system and enabling features in documents.

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

class UIDictationPhrase

An object that represents the textual interpretation of a spoken phrase that the user dictates.

