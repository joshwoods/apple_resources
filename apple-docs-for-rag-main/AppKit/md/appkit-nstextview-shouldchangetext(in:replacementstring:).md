

- AppKit
- NSTextView
-  shouldChangeText(in:replacementString:) 

Instance Method

# shouldChangeText(in:replacementString:)

Initiates a series of delegate messages (and general notifications) to determine whether modifications can be made to the characters and attributes of the receiver’s text.

macOS

``` source
@MainActor
func shouldChangeText(
    in affectedCharRange: NSRange,
    replacementString: String?
) -> Bool
```

## Parameters 

`affectedCharRange`  

The range of characters affected by the proposed change.

`replacementString`  

The characters that will replace those in `affectedCharRange`. If only text attributes are being changed, `replacementString` is `nil`.

## Return Value

true to allow the change, false to prohibit it.

## Discussion

This method checks with the delegate as needed using textShouldBeginEditing(_:) and textView(_:shouldChangeTextIn:replacementString:).

This method must be invoked at the start of any sequence of user-initiated editing changes. If your subclass of `NSTextView` implements methods that modify the text, make sure to invoke this method to determine whether the change should be made. If the change is allowed, complete the change by invoking the didChangeText() method.

### Special Considerations

If you override this method, you must call `super` at the beginning of the override.

If the receiver is not editable, this method automatically returns false. This result prevents instances in which a text view could be changed by user actions even though it had been set to be non-editable.

In macOS 10.4 and later, if there are multiple selections, this method acts on the first selected subrange.

## See Also

### Related Documentation

var isEditable: Bool

A Boolean value that controls whether the text views sharing the receiver’s layout manager allow the user to edit text.

### Customizing subclass behaviors

func updateFontPanel()

Updates the Font panel to contain the font attributes of the selection.

func updateRuler()

Updates the ruler view in the receiver’s enclosing scroll view to reflect the selection’s paragraph and marker attributes.

var acceptableDragTypes: [NSPasteboard.PasteboardType]

The data types that the receiver accepts as the destination view of a dragging operation.

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

func shouldChangeText(inRanges: [NSValue], replacementStrings: [String]?) -> Bool

Initiates a series of delegate messages (and general notifications) to determine whether modifications can be made to the characters and attributes of the receiver’s text.

func didChangeText()

Sends out necessary notifications when a text change completes.

var smartInsertDeleteEnabled: Bool

A Boolean value that controls whether the receiver inserts or deletes space around selected words so as to preserve proper spacing and punctuation.

func smartDeleteRange(forProposedRange: NSRange) -> NSRange

Returns an extended range that includes adjacent whitespace that should be deleted along with the proposed range in order to preserve proper spacing and punctuation.

