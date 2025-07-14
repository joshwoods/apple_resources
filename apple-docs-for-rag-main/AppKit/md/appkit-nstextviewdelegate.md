

- AppKit
-  NSTextViewDelegate 

Protocol

# NSTextViewDelegate

A set of optional methods that text view delegates can use to manage selection, set text attributes, work with the spell checker, and more.

macOS

``` source
protocol NSTextViewDelegate : NSTextDelegate
```

## Topics

### Accessing Text System Objects

func undoManager(for: NSTextView) -> UndoManager?

Returns the undo manager for the specified text view.

### Controlling Display

func textView(NSTextView, willDisplayToolTip: String, forCharacterAt: Int) -> String?

Returns the actual tooltip to display.

### Supporting Quick Look

func textView(NSTextView, urlForContentsOf: NSTextAttachment, at: Int) -> URL?

Returns a URL representing the document contents for a text attachment.

### Managing the Selection

func textView(NSTextView, willChangeSelectionFromCharacterRange: NSRange, toCharacterRange: NSRange) -> NSRange

Returns the actual range to select.

func textView(NSTextView, willChangeSelectionFromCharacterRanges: [NSValue], toCharacterRanges: [NSValue]) -> [NSValue]

Returns the actual character ranges to select.

func textViewDidChangeSelection(Notification)

Sent when the selection changes in the text view.

func textView(NSTextView, candidates: [NSTextCheckingResult], forSelectedRange: NSRange) -> [NSTextCheckingResult]

Returns an array of text objects to include in a text selection.

func textView(NSTextView, candidatesForSelectedRange: NSRange) -> [Any]?

Returns an array of objects that represent the elements of a selection.

func textView(NSTextView, shouldSelectCandidateAt: Int) -> Bool

Returns a Boolean value that indicates whether to select the text object at the index.

func textView(NSTextView, shouldUpdateTouchBarItemIdentifiers: [NSTouchBarItem.Identifier]) -> [NSTouchBarItem.Identifier]

Returns and array of touch bar elements for the framework to update.

### Managing the Pasteboard

func textView(NSTextView, writablePasteboardTypesFor: any NSTextAttachmentCellProtocol, at: Int) -> [NSPasteboard.PasteboardType]

Returns the writable pasteboard types for a given cell.

func textView(NSTextView, write: any NSTextAttachmentCellProtocol, at: Int, to: NSPasteboard, type: NSPasteboard.PasteboardType) -> Bool

Returns whether data of the specified type for the given cell could be written to the specified pasteboard.

### Setting Text Attributes

func textView(NSTextView, shouldChangeTextIn: NSRange, replacementString: String?) -> Bool

Sent when a text view needs to determine if text in a specified range should be changed.

func textView(NSTextView, shouldChangeTextInRanges: [NSValue], replacementStrings: [String]?) -> Bool

Sent when a text view needs to determine if text in an array of specified ranges should be changed.

func textView(NSTextView, shouldChangeTypingAttributes: [String : Any], toAttributes: [NSAttributedString.Key : Any]) -> [NSAttributedString.Key : Any]

Sent when the typing attributes are changed.

func textViewDidChangeTypingAttributes(Notification)

Sent when a text view’s typing attributes change.

### Clicking and Pasting

func textView(NSTextView, clickedOn: any NSTextAttachmentCellProtocol, in: NSRect, at: Int)

Sent when the user clicks a cell.

func textView(NSTextView, doubleClickedOn: any NSTextAttachmentCellProtocol, in: NSRect, at: Int)

Sent when the user double-clicks a cell.

func textView(NSTextView, clickedOnLink: Any, at: Int) -> Bool

Sent after the user clicks a link.

### Working With the Spelling Checker

func textView(NSTextView, shouldSetSpellingState: Int, range: NSRange) -> Int

Sent when the spelling state is changed.

func textView(NSTextView, willCheckTextIn: NSRange, options: [NSSpellChecker.OptionKey : Any], types: UnsafeMutablePointer&lt;NSTextCheckingTypes>) -> [NSSpellChecker.OptionKey : Any]

Invoked to allow the delegate to modify the text checking process before it occurs.

func textView(NSTextView, didCheckTextIn: NSRange, types: NSTextCheckingTypes, options: [NSSpellChecker.OptionKey : Any], results: [NSTextCheckingResult], orthography: NSOrthography, wordCount: Int) -> [NSTextCheckingResult]

Invoked to allow the delegate to modify the text checking results after checking has occurred.

### Responding to writing tools interactions

func textViewWritingToolsWillBegin(NSTextView)

func textViewWritingToolsDidEnd(NSTextView)

func textView(NSTextView, writingToolsIgnoredRangesInEnclosingRange: NSRange) -> [NSValue]

### Dragging

func textView(NSTextView, draggedCell: any NSTextAttachmentCellProtocol, in: NSRect, event: NSEvent, at: Int)

Sent when the user attempts to drag a cell.

### Completing text

func textView(NSTextView, completions: [String], forPartialWordRange: NSRange, indexOfSelectedItem: UnsafeMutablePointer&lt;Int>?) -> [String]

Returns the actual completions for a partial word.

### Displaying the sharing service picker

func textView(NSTextView, willShow: NSSharingServicePicker, forItems: [Any]) -> NSSharingServicePicker?

Returns a sharing service picker for the current selection.

### Performing Commands

func textView(NSTextView, doCommandBy: Selector) -> Bool

Sent to allow the delegate to perform the command for the text view.

### Contextual Menu Management

func textView(NSTextView, menu: NSMenu, for: NSEvent, at: Int) -> NSMenu?

Allows delegate to control the context menu returned by the text view.

## Relationships

### Inherits From

- NSObjectProtocol
- NSTextDelegate

### Conforming Types

- NSOutlineView
- NSTableView

## See Also

### Text views

class NSTextField

Text the user can select or edit to send an action message to a target when the user presses the Return key.

protocol NSTextFieldDelegate

A protocol that a text field delegate can use to control its field editor action menu.

class NSTextView

A view that draws text and handles user interactions with that text.

protocol NSTextDelegate

A set of optional methods implemented by the delegate of an NSText object to edit text and change text formats.

class NSText

The most general programmatic interface for objects that manage text.

