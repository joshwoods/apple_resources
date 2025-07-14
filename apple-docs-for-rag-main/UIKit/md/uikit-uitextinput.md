

- UIKit
-  UITextInput 

Protocol

# UITextInput

A set of methods for interacting with the text input system and enabling features in documents.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
protocol UITextInput : UIKeyInput
```

## Mentioned in 

Adopting system selection UI in custom text views

Adopting Smart Reply in your messaging or email app

## Overview

Objects that adopt the UITextInput protocol maintain information about text input and provide that information to the text input system on demand. A UITextInput object interacts with the text input system by:

- Reporting text positions and text ranges

- Responding to queries layout and writing direction

- Performing hit-testing — returning text positions and ranges for a specific point

- Providing the system with rectangles for highlighting ranges of text and drawing the *caret*, a glyph that represents the insertion point during text entry

In addition, a UITextInput object maintains ranges for selected text and marked text. Marked text, a part of multistage text input, represents provisionally inserted text that the user has yet to confirm. The range of marked text always contains a range of selected text, which might be a range of characters or the caret. Multistage text input is a requirement when the language is ideographic and the keyboard is phonetic.

### Integrate with the text input system

The UITextInput protocol works with other classes and protocols to integrate text-processing apps with the text input system:

UITextPosition and UITextRange classes  
All UITextInput-conforming document classes must create custom subclasses of these classes. A UITextPosition object represents a position in a text container. A UITextRange object, which encapsulates beginning and ending UITextPosition objects, represents a range of characters in the text container.

UITextInputTokenizer protocol and UITextInputStringTokenizer class  
The UITextInputTokenizer protocol defines an interface for tokenizing input text. The UITextInputStringTokenizer class is a default implementation of this protocol.

UITextInputDelegate protocol  
The text input system automatically assigns its own text input delegate (which conforms to this protocol) to the UITextInput-conforming document object. This text input delegate allows document objects to inform the input system of changes in text and selection.

UIKeyInput protocol  
Implement this protocol to allow text entry and deletion at an insertion point.

### Customize keyboard behavior

The UITextInput protocol also inherits the UITextInputTraits protocol, which provides customization of the keyboard and its behaviors.

When the user chooses dictation input on a supported device, the system automatically inserts recognized phrases into the current text view. Methods in the UITextInput protocol allow your app to respond to the completion of dictation. You can use an object of the UIDictationPhrase class to obtain a string that represents a phrase the user dictates. In the case of ambiguous dictation results, a dictation phrase object provides an array that contains alternative strings.

## Topics

### Handling text input

var inputDelegate: (any UITextInputDelegate)?

An input delegate that receives a notification when text changes or when the selection changes.

**Required**

protocol UITextInputDelegate

An intermediary between a document and the text input system.

### Replacing and returning text

func text(in: UITextRange) -> String?

Returns the text in the specified range.

**Required**

func replace(UITextRange, withText: String)

Replaces the text in a document that is in the specified range.

**Required**

func shouldChangeText(in: UITextRange, replacementText: String) -> Bool

Asks whether to replace the text in the specified range.

### Working with marked and selected text

var selectedTextRange: UITextRange?

The range of selected text in a document.

**Required**

var markedTextRange: UITextRange?

The range of currently marked text in a document.

**Required**

var markedTextStyle: [NSAttributedString.Key : Any]?

A dictionary of attributes that describes how to draw marked text.

**Required**

func setMarkedText(String?, selectedRange: NSRange)

Inserts the provided text and marks it to indicate that it is part of an active input session.

**Required**

func setAttributedMarkedText(NSAttributedString?, selectedRange: NSRange)

Inserts the provided styled text and marks it to indicate that it is part of an active input session.

func unmarkText()

Unmarks the currently marked text.

**Required**

var selectionAffinity: UITextStorageDirection

The desired location for the insertion point.

### Computing text ranges and text positions

func textRange(from: UITextPosition, to: UITextPosition) -> UITextRange?

Returns the range between two text positions.

**Required**

func position(from: UITextPosition, offset: Int) -> UITextPosition?

Returns the text position at a specified offset from another text position.

**Required**

func position(from: UITextPosition, in: UITextLayoutDirection, offset: Int) -> UITextPosition?

Returns the text position at a specified offset in a specified direction from another text position.

**Required**

var beginningOfDocument: UITextPosition

The text position for the beginning of a document.

**Required**

var endOfDocument: UITextPosition

The text position for the end of a document.

**Required**

### Evaluating text positions

func compare(UITextPosition, to: UITextPosition) -> ComparisonResult

Returns how one text position compares to another text position.

**Required**

func offset(from: UITextPosition, to: UITextPosition) -> Int

Returns the number of UTF-16 characters between one text position and another text position.

**Required**

### Making the view non-editable

var isEditable: Bool

A Boolean value that indicates whether the text view contains editable text.

### Determining layout and writing direction

func position(within: UITextRange, farthestIn: UITextLayoutDirection) -> UITextPosition?

Returns the text position that is at the farthest extent in a specified layout direction within a range of text.

**Required**

func characterRange(byExtending: UITextPosition, in: UITextLayoutDirection) -> UITextRange?

Returns a text range from a specified text position to its farthest extent in a certain direction of layout.

**Required**

func baseWritingDirection(for: UITextPosition, in: UITextStorageDirection) -> NSWritingDirection

Returns the base writing direction for a position in the text going in a certain direction.

**Required**

func setBaseWritingDirection(NSWritingDirection, for: UITextRange)

Sets the base writing direction for a specified range of text in a document.

**Required**

### Working with geometry and hit-testing

func firstRect(for: UITextRange) -> CGRect

Returns the first rectangle that encloses a range of text in a document.

**Required**

func closestPosition(to: CGPoint) -> UITextPosition?

Returns the position in a document that is closest to a specified point.

**Required**

func selectionRects(for: UITextRange) -> [UITextSelectionRect]

Returns an array of selection rects corresponding to the range of text.

**Required**

func closestPosition(to: CGPoint, within: UITextRange) -> UITextPosition?

Returns the position in a document that is closest to a specified point in a specified range.

**Required**

func characterRange(at: CGPoint) -> UITextRange?

Returns the character or range of characters that is at a specified point in a document.

**Required**

### Providing the caret layout information

func caretRect(for: UITextPosition) -> CGRect

Returns a rectangle to draw the caret at a specified insertion point.

**Required**

func caretTransform(for: UITextPosition) -> CGAffineTransform

Returns the transform to apply to the caret prior to drawing.

### Tokenizing input text

var tokenizer: any UITextInputTokenizer

An input tokenizer that provides information about the granularity of text units.

**Required**

protocol UITextInputTokenizer

A tokenizer, which is an object that allows the text input system to evaluate text units of different granularities.

### Managing the floating cursor

func beginFloatingCursor(at: CGPoint)

Tells the object when the gesture that the system uses to manipulate the cursor begins.

func updateFloatingCursor(at: CGPoint)

Tells the object that the floating cursor moved to a new location.

func endFloatingCursor()

Tells the object when the gesture that the system uses to manipulate the cursor ends.

### Using dictation

func dictationRecordingDidEnd()

Tells the object when there is a pending dictation result.

func dictationRecognitionFailed()

Tells the object when dictation ends, but recognition fails.

func insertDictationResult([UIDictationPhrase])

Tells the object when there is more than one interpretation of a spoken phrase in a dictation result.

var insertDictationResultPlaceholder: Any

Asks for the placeholder object to use while generating dictation results.

func frame(forDictationResultPlaceholder: Any) -> CGRect

Asks for the rectangle for displaying the dictation placeholder animation.

func removeDictationResultPlaceholder(Any, willInsertResult: Bool)

Tells the view that the specified placeholder object is unnecessary.

### Managing placeholders

func insertTextPlaceholder(with: CGSize) -> UITextPlaceholder

Inserts a placeholder object to reserve visual space during text input.

func remove(UITextPlaceholder)

Removes a placeholder object from the text input view.

class UITextPlaceholder

A placeholder object that reserves visual space in a text input view.

### Managing the edit menu

func editMenu(for: UITextRange, suggestedActions: [UIMenuElement]) -> UIMenu?

Asks for the menu to display for the given text range and actions the system provides.

func willPresentEditMenu(animator: any UIEditMenuInteractionAnimating)

Tells the object when the system is about to present an edit menu with an animator.

func willDismissEditMenu(animator: any UIEditMenuInteractionAnimating)

Tells the object when the system is about to dismiss an edit menu with an animator.

### Supporting text-phrase alternatives

func insertText(String, alternatives: [String], style: UITextAlternativeStyle)

enum UITextAlternativeStyle

A constant that determines if the system highlights alternative phrases during text input.

### Inserting a Smart Reply suggestion

func insert(UIInputSuggestion)

Inserts the user or system’s input suggestion into the document.

### Supporting adaptive images

var supportsAdaptiveImageGlyph: Bool

A Boolean value that indicates whether the document supports adaptive images in the input.

func insert(NSAdaptiveImageGlyph, replacementRange: UITextRange)

Inserts an adaptive image into the text at the specifed location.

### Returning text-styling information

func textStyling(at: UITextPosition, in: UITextStorageDirection) -> [NSAttributedString.Key : Any]?

Returns a dictionary with properties that specify how to style the text at a certain location in a document.

### Reconciling text position and character offset

func position(within: UITextRange, atCharacterOffset: Int) -> UITextPosition?

Returns the position within a range of a document’s text that corresponds to the character offset from the start of that range.

func characterOffset(of: UITextPosition, within: UITextRange) -> Int

Returns the character offset of a position in a document’s text that falls within a specified range.

### Returning the text input view

var textInputView: UIView

An affiliated view that provides a coordinate system for all geometric values in the protocol.

### Constants

struct UITextDirection

The direction of the text.

enum UITextStorageDirection

The direction of text storage.

enum UITextLayoutDirection

The direction of text layout.

### Deprecated

typealias UITextWritingDirection

The writing direction of the text for the language.

Deprecated

Style dictionary keys

A dictionary that contains properties that define text style characteristics.

### Instance Methods

func attributedText(in: UITextRange) -> NSAttributedString

func didDismissWritingTools()

func insertAttributedText(NSAttributedString)

func replace(UITextRange, withAttributedText: NSAttributedString)

func willPresentWritingTools()

## Relationships

### Inherits From

- NSObjectProtocol
- UIKeyInput
- UITextInputTraits

### Inherited By

- UITextDraggable
- UITextDroppable

### Conforming Types

- UISearchTextField
- UITextField
- UITextView

## See Also

### Text input

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

class UIDictationPhrase

An object that represents the textual interpretation of a spoken phrase that the user dictates.

