

- BrowserEngineKit
-  BETextInput 

Protocol

# BETextInput

A protocol to which text views conform to asynchronously integrate with the text system.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
protocol BETextInput : BEResponderEditActions, BETextSelectionDirectionNavigation, UIKeyInput
```

## Mentioned in 

Integrating custom browser text views with UIKit

Supporting extended text interactions

## Overview

You adopt `BETextInput` in your text field when you need to perform asynchronous actions to provide information for the text system, for example, making an XPC request to a web content extension. For more information, see Integrating custom browser text views with UIKit.

## Topics

### Updating the text system

var asyncInputDelegate: (any BETextInputDelegate)?

A system-provided input delegate is assigned when the system is interested in input changes.

**Required**

func canPerformAction(Selector, withSender: Any?) -> Bool

Returns whether text related actions, such those included in UIResponderStandardEditActions, can be handled

**Required**

### Handling text input

var isEditable: Bool

Reflects the ability to modify text

**Required**

func handleKeyEntry(BEKeyEntry, completionHandler: (BEKeyEntry, Bool) -> Void)

Accepts key-entry events from the text system for the text view to process.

**Required**

func shiftKeyStateChanged(fromState: BEKeyModifierFlags, toState: BEKeyModifierFlags)

Indicates a transition in shift state

**Required**

func text(in: UITextRange) -> String?

Returns the text in the specified range.

**Required**

func offset(from: UITextPosition, to: UITextPosition) -> Int

Returns the number of UTF-16 characters between one text position and another text position.

**Required**

func setBaseWritingDirection(NSWritingDirection, for: UITextRange)

Sets the base writing direction for a specified range of text in a document.

**Required**

func delete(in: UITextStorageDirection, to: UITextGranularity)

Deletes text by the specified direction and granularity. Current supported combinations include:

**Required**

### Editing and correcting text

func transposeCharactersAroundSelection()

Transposes the characters on either side of the caret in response to the key command, ctrl + T

**Required**

func replaceText(String, withText: String, options: BETextReplacementOptions, completionHandler: ([UITextSelectionRect]) -> Void)

Replace the specified text preceding the current selection.

**Required**

func requestTextContextForAutocorrection(completionHandler: (BETextDocumentContext) -> Void)

Invoked by the system to gather context around the current selection. Clients should generally include the setence that contains the current selection and include the previous sentence if the current selection is at a boundary.

**Required**

func requestTextRects(for: String, withCompletionHandler: ([UITextSelectionRect]) -> Void)

Invoked by the system to gather context for the presentation of various text related UI’s. Completion handler should be invoked with the `UITextSelectionRect`s for the substring nearest to the caret that matches the given `input`

**Required**

var automaticallyPresentEditMenu: Bool

Controls whether the edit menu is allowed to be presented or should be suppressed.

**Required**

func requestPreferredArrowDirectionForEditMenu(completionHandler: (UIEditMenuArrowDirection) -> Void)

Invoked by the system to gather context, including the client’s preference for how the edit menu should be positioned relative to the selected text.

**Required**

func systemWillPresentEditMenu(withAnimator: any UIEditMenuInteractionAnimating)

Invoked by the system when it is about to present an edit menu with an animator.

**Required**

func systemWillDismissEditMenu(withAnimator: any UIEditMenuInteractionAnimating)

Invoked by the system when it is about to dismiss an edit menu with an animator.

**Required**

### Input traits

var extendedTextInputTraits: (any BEExtendedTextInputTraits)?

Object from which the BEExtendedTextInputTraits will be gathered.

**Required**

func textStyling(at: UITextPosition, in: UITextStorageDirection) -> [NSAttributedString.Key : Any]?

Returns a dictionary containing NSAttributedString keys represeting appearance customizations.

**Required**

### Replacing text

var isReplaceAllowed: Bool

Returns whether replacement should be allowed for an editable element.

**Required**

func replaceSelectedText(String, withText: String)

Replaces the specified `text` with `replacementText`

**Required**

### Handling text gestures

func updateCurrentSelection(to: CGPoint, from: BEGestureType, in: UIGestureRecognizer.State)

Indicates the `point` the text interaction gesture is tracking has changed

**Required**

func setSelection(from: CGPoint, to: CGPoint, gesture: BEGestureType, state: UIGestureRecognizer.State)

Notifies the text view that its selection needs to change to the text between the given points.

**Required**

func adjustSelectionBoundary(to: CGPoint, touchPhase: BESelectionTouchPhase, baseIsStart: Bool, flags: BESelectionFlags)

Adjusts the selection’s start or end boundary specified by `boundaryIsStart` to the `point`

**Required**

func textInteractionGesture(BEGestureType, shouldBeginAt: CGPoint) -> Bool

Returns whether a gesture with the given `gestureType` should begin for the given `point`

**Required**

### Selecting text

var selectedText: String?

String representing the selected text.

**Required**

var selectedTextRange: UITextRange?

Range representing the selected text.

**Required**

var isSelectionAtDocumentStart: Bool

Represents whether the current selection is at the beginning of the document

**Required**

func caretRect(for: UITextPosition) -> CGRect

Returns a rectangle to draw the caret at a specified insertion point.

**Required**

func selectionRects(for: UITextRange) -> [UITextSelectionRect]

Returns an array of selection rects corresponding to the range of text.

**Required**

func selectWordForReplacement()

Selects a word with autocorrect replacement suggestions when it is tapped

**Required**

func updateSelection(extent: CGPoint, boundary: UITextGranularity, completionHandler: (Bool) -> Void)

Includes the text up to the given point in the current text selection.

**Required**

func selectText(in: UITextGranularity, at: CGPoint, completionHandler: () -> Void)

Selects the text within the given granularity at the given point in the text view.

**Required**

func selectPosition(at: CGPoint, completionHandler: () -> Void)

Sets the selection caret to the given point

**Required**

func selectPosition(at: CGPoint, for: BETextDocumentRequest, completionHandler: (BETextDocumentContext) -> Void)

Sets the selection caret to the given point. Also includes a convenience document context request.

**Required**

func adjustSelection(by: BEDirectionalTextRange, completionHandler: () -> Void)

Adjusts the selection by the moving the selected range by the given `range`, in character granularity units.

**Required**

func move(byOffset: Int)

Adjusts the current selection by `offset` in character granularity units

**Required**

func moveSelection(atBoundary: UITextGranularity, in: UITextStorageDirection, completionHandler: () -> Void)

Moves the caret to relative to the current position in the `direction` to the given `granularity`. The `direction` is “forward” or “backward” in accordance with the directionality of the language.

**Required**

func selectTextForEditMenuWithLocation(inView: CGPoint, completionHandler: (Bool, String?, NSRange) -> Void)

Indicates the edit menu is being shown at the given location in the text input view’s coordinate space.

**Required**

### Marking text

var markedText: String?

String for the text that has been marked as part of an active input session

**Required**

var attributedMarkedText: NSAttributedString?

Attributed string for the text that has been marked as part of an active input session

**Required**

var markedTextRange: UITextRange?

Range representing the position of the markedText.

**Required**

var hasMarkedText: Bool

Indicates whether there any text is currently marked as part of an active input session

**Required**

func setMarkedText(String?, selectedRange: NSRange)

Inserts the provided text and marks it to indicate that it is part of an active input session.

**Required**

func setAttributedMarkedText(NSAttributedString?, selectedRange: NSRange)

Inserts the provided styled text and marks it to indicate that it is part of an active input session.

**Required**

func unmarkText()

Unmarks the currently marked text

**Required**

func isPointNearMarkedText(CGPoint) -> Bool

Returns whether a point should be considered “near” the marked text. Used to determine whether text interaction gestures near marked text should begin.

**Required**

### Document context

func requestDocumentContext(BETextDocumentRequest, completionHandler: (BETextDocumentContext) -> Void)

Gathers context about the current document for the system

**Required**

### Dictation

func willInsertFinalDictationResult()

Indicates the system is about to insert the final dictation result.

**Required**

func replaceDictatedText(String, withText: String)

Inserts/replaces text for a dictation.

**Required**

func didInsertFinalDictationResult()

Indicates system has inserted the final dictation result

**Required**

### Text alternatives

func alternativesForSelectedText() -> [BETextAlternatives]?

Returns the text alternatives that are available to the text input object.

**Required**

func add(BETextAlternatives)

Adds text alternatives to the text input object for the current selection

**Required**

func insert(BETextAlternatives)

Inserts the given `text` or one of it’s alternative texts available on `alternatives`

**Required**

### Text placeholders

func insertTextPlaceholder(size: CGSize, completionHandler: (UITextPlaceholder) -> Void)

Inserts a placeholder object to reserve visual space during text input. If `size.height` is less than or equal to zero, then the placeholder is inline and line height. If `size.height` is greather than zero, then the placeholder is treated as a paragraph of height `size.height`.

**Required**

func remove(UITextPlaceholder, willInsertText: Bool, completionHandler: () -> Void)

Removes a placeholder object from the text input view.

**Required**

### Text suggestions

func insert(BETextSuggestion)

Inserts a `textSuggestion` in response to a user suggestion selection

**Required**

### Geometry

var textInputView: UIView

An affiliated view that provides a coordinate system for all geometric values in this protocol.

**Required**

var textFirstRect: CGRect

Returns a rect representing the bounds of the first line of marked text, if marked text is set.

**Required**

var textLastRect: CGRect

Returns a rect representing the bounds of the last line of marked text, if marked text is set.

**Required**

var unobscuredContentRect: CGRect

Rect used to place UI (such as selection handles) in a location that isn’t obscurred by app UI.

**Required**

var unscaledView: UIView

View representing the web content that is agnostic of zoom state. Used to draw zoom agnostic system UI elements, such as the selection handles

**Required**

var selectionClipRect: CGRect

Rect representing the bounds of editable elements, used to ensure and UI don’t overflow outside them

**Required**

func autoscroll(to: CGPoint)

Indicates autoscrolling has been triggered by a text interaction gesture.

**Required**

func cancelAutoscroll()

Indicates autoscrolling is complete.

**Required**

### Instance Methods

func keyboardWillDismiss()

Called when the user has requested the keyboard to dismiss itself.

func removeTextAlternatives()

Removes text alternatives from the text input object for the current selection

## Relationships

### Inherits From

- BEResponderEditActions
- BETextSelectionDirectionNavigation
- NSObjectProtocol
- UIKeyInput
- UIResponderStandardEditActions
- UITextInputTraits

## See Also

### Custom text views

Integrating custom browser text views with UIKit

Process keyboard interactions asynchronously in your iOS browser app’s text view.

Supporting extended text interactions

Share content, add replacement shortcuts, and perform other rich actions in browser text views.

protocol BETextInputDelegate

A delegate protocol that a browser text view uses to notify the text system of changes.

