

- UIKit
-  UITextDocumentProxy 

Protocol

# UITextDocumentProxy

An object that provides textual context to a custom keyboard.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
protocol UITextDocumentProxy : UIKeyInput
```

## Mentioned in 

Handling text interactions in custom keyboards

## Overview

Through conformance to the UIKeyInput protocol, a text document proxy enables a custom keyboard (which is based on the UIInputViewController class) to insert and delete text, to adjust the position of the insertion point, and to determine whether a text input object is empty. The text document proxy uses the keyboard’s textDocumentProxy property to do this.

For more about using a text document proxy, see UIInputViewController and Creating a custom keyboard.

## Topics

### Getting the text-input mode

var documentInputMode: UITextInputMode?

The text-input mode for the keyboard.

**Required**

### Obtaining textual context around the insertion point

var documentContextAfterInput: String?

Textual context after the insertion point in the current text input object.

**Required**

var documentContextBeforeInput: String?

Textual context before the insertion point in the current text input object.

**Required**

### Adjusting the insertion point position

func adjustTextPosition(byCharacterOffset: Int)

Moves the insertion point forward or backward in the current text input object.

**Required**

### Getting the selected text

var selectedText: String?

The currently selected text in the document.

**Required**

### Managing marked text

func setMarkedText(String, selectedRange: NSRange)

Inserts the provided text and marks it to indicate that it’s part of an active input session.

**Required**

func unmarkText()

Unmarks the currently marked text.

**Required**

### Distinguishing changes in the document

var documentIdentifier: UUID

The unique identifier for the document.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol
- UIKeyInput
- UITextInputTraits

## See Also

### Custom keyboard

protocol UIInputViewAudioFeedback

A property that enables a custom input or keyboard accessory view to play standard keyboard input clicks.

class UIInputViewController

The primary view controller for a custom keyboard app extension.

class UILexicon

A read-only array of term pairs, each in a lexicon entry object, for a custom keyboard.

class UILexiconEntry

A read-only term pair, available within a lexicon object, for a custom keyboard.

