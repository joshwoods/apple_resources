

- AppKit
- NSTextView
-  selectionRange(forProposedRange:granularity:) 

Instance Method

# selectionRange(forProposedRange:granularity:)

Returns an adjusted selected range based on the selection granularity.

macOS

``` source
@MainActor
func selectionRange(
    forProposedRange proposedCharRange: NSRange,
    granularity: NSSelectionGranularity
) -> NSRange
```

## Parameters 

`proposedCharRange`  

The proposed selected range.

`granularity`  

The selection granularity.

## Return Value

The adjusted selected range, taking into account the selection granularity.

## Discussion

This method is invoked repeatedly during mouse tracking to modify the range of the selection. Override this method to specialize selection behavior.

## See Also

### Related Documentation

var selectionGranularity: NSSelectionGranularity

The selection granularity for subsequent extension of a selection.

### Customizing subclass behaviors

func updateFontPanel()

Updates the Font panel to contain the font attributes of the selection.

func updateRuler()

Updates the ruler view in the receiver’s enclosing scroll view to reflect the selection’s paragraph and marker attributes.

var acceptableDragTypes: [NSPasteboard.PasteboardType]

The data types that the receiver accepts as the destination view of a dragging operation.

func updateDragTypeRegistration()

Updates the acceptable drag types of all text views associated with the receiver’s layout manager.

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

