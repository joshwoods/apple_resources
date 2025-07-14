

- UIKit
-  UIKeyInput 

Protocol

# UIKeyInput

A set of methods a responder uses to implement simple text entry.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
protocol UIKeyInput : UITextInputTraits
```

## Mentioned in 

Handling text interactions in custom keyboards

## Overview

Adopt this protocol in a subclass of UIResponder to support text entry. When instances of this subclass are the first responder, the system keyboard displays. Only a small subset of the available keyboards and languages are available to classes that adopt this protocol.

## Topics

### Inserting and deleting text

func insertText(String)

Inserts a character into the displayed text.

**Required**

func deleteBackward()

Deletes a character from the displayed text.

**Required**

var hasText: Bool

A Boolean value that indicates whether the text-entry object has any text.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol
- UITextInputTraits

### Inherited By

- UITextDocumentProxy
- UITextDraggable
- UITextDroppable
- UITextInput

### Conforming Types

- UISearchTextField
- UITextField
- UITextView

## See Also

### Text input

protocol UITextInput

A set of methods for interacting with the text input system and enabling features in documents.

protocol UITextInputDelegate

An intermediary between a document and the text input system.

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

