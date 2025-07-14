

- AppKit
- NSTextView
-  acceptableDragTypes 

Instance Property

# acceptableDragTypes

The data types that the receiver accepts as the destination view of a dragging operation.

macOS

``` source
@MainActor
var acceptableDragTypes: [NSPasteboard.PasteboardType] { get }
```

## Discussion

These types are automatically registered as necessary by the text view. Subclasses should override this value as necessary to add their own types to those returned by `NSTextView`‘s implementation. They must then also override the appropriate methods of the NSDraggingDestination protocol to support import of those types. See that protocol’s specification for more information.

## See Also

### Customizing subclass behaviors

func updateFontPanel()

Updates the Font panel to contain the font attributes of the selection.

func updateRuler()

Updates the ruler view in the receiver’s enclosing scroll view to reflect the selection’s paragraph and marker attributes.

func updateDragTypeRegistration()

Updates the acceptable drag types of all text views associated with the receiver’s layout manager.

func selectionRange(forProposedRange: NSRange, granularity: NSSelectionGranularity) -> NSRange

Returns an adjusted selected range based on the selection granularity.

var rangeForUserCharacterAttributeChange: NSRange

The range of characters affected by an action method that changes character (not paragraph) attributes.

var rangesForUserCharacterAttributeChange: [NSValue]?

An array containing the ranges of characters affected by an action method that changes character (not paragraph) attributes.

var rangeForUserParagraphAttributeChange: NSRange

The range of characters affected by an action method that changes paragraph (not character) attributes.

var rangesForUserParagraphAttributeChange: [NSValue]?

An array containing the ranges of characters affected by a method that changes paragraph (not character) attributes.

var rangeForUserTextChange: NSRange

The range of characters affected by a method that changes characters (as opposed to attributes).

var rangesForUserTextChange: [NSValue]?

An array containing the ranges of characters affected by a method that changes characters (as opposed to attributes).

func shouldChangeText(in: NSRange, replacementString: String?) -> Bool

Initiates a series of delegate messages (and general notifications) to determine whether modifications can be made to the characters and attributes of the receiver’s text.

func shouldChangeText(inRanges: [NSValue], replacementStrings: [String]?) -> Bool

Initiates a series of delegate messages (and general notifications) to determine whether modifications can be made to the characters and attributes of the receiver’s text.

func didChangeText()

Sends out necessary notifications when a text change completes.

var smartInsertDeleteEnabled: Bool

A Boolean value that controls whether the receiver inserts or deletes space around selected words so as to preserve proper spacing and punctuation.

func smartDeleteRange(forProposedRange: NSRange) -> NSRange

Returns an extended range that includes adjacent whitespace that should be deleted along with the proposed range in order to preserve proper spacing and punctuation.

