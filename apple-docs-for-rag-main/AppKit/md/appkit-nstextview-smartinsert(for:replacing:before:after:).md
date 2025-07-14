

- AppKit
- NSTextView
-  smartInsert(for:replacing:before:after:) 

Instance Method

# smartInsert(for:replacing:before:after:)

Determines whether whitespace needs to be added around the string to preserve proper spacing and punctuation when it replaces the characters in the specified range.

macOS

``` source
@MainActor
func smartInsert(
    for pasteString: String,
    replacing charRangeToReplace: NSRange,
    before beforeString: AutoreleasingUnsafeMutablePointer?,
    after afterString: AutoreleasingUnsafeMutablePointer?
)
```

## Parameters 

`pasteString`  

The string that is replacing the characters in `charRange`.

`charRangeToReplace`  

The range of characters which `aString` is replacing.

`beforeString`  

On return, a pointer to the string with the characters that should be added before `aString`; `nil` if there are no characters to add, if `aString` is `nil`, or if smart insertion and deletion are disabled.

`afterString`  

On return, a pointer to the string with the characters that should be added after `aString`; `nil` if there are no characters to add, if `aString` is `nil`, or if smart insertion and deletion are disabled.

## Discussion

As part of its implementation, this method calls smartInsert(afterStringFor:replacing:) and smartInsert(beforeStringFor:replacing:). To change this method’s behavior, override those two methods instead of this one.

`NSTextView` uses this method as necessary. You can also use it in implementing your own methods that insert text. To do so, invoke this method with the proper arguments, then insert `beforeString`, `aString`, and `afterString` in order over `charRange`.

## See Also

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

func shouldChangeText(in: NSRange, replacementString: String?) -> Bool

Initiates a series of delegate messages (and general notifications) to determine whether modifications can be made to the characters and attributes of the receiver’s text.

func shouldChangeText(inRanges: [NSValue], replacementStrings: [String]?) -> Bool

Initiates a series of delegate messages (and general notifications) to determine whether modifications can be made to the characters and attributes of the receiver’s text.

func didChangeText()

Sends out necessary notifications when a text change completes.

var smartInsertDeleteEnabled: Bool

A Boolean value that controls whether the receiver inserts or deletes space around selected words so as to preserve proper spacing and punctuation.

