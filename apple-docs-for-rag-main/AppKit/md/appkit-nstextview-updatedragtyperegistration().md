

- AppKit
- NSTextView
-  updateDragTypeRegistration() 

Instance Method

# updateDragTypeRegistration()

Updates the acceptable drag types of all text views associated with the receiver’s layout manager.

macOS

``` source
@MainActor
func updateDragTypeRegistration()
```

## Discussion

If the receiver is editable and is a rich text view, causes all text views associated with the receiver’s layout manager to register their acceptable drag types. If the text view isn’t editable or isn’t rich text, causes those text views to unregister their dragged types.

Subclasses can override this method to change the conditions for registering and unregistering drag types, whether as a group or individually based on the current state of the text view. They should invoke this method when that state changes to perform the necessary update.

## See Also

### Related Documentation

func registerForDraggedTypes([NSPasteboard.PasteboardType])

Registers the pasteboard types that the view will accept as the destination of an image-dragging session.

func unregisterDraggedTypes()

Unregisters the view as a possible destination in a dragging session.

var importsGraphics: Bool

A Boolean value that controls whether the text views sharing the receiver’s layout manager allow the user to import files by dragging.

var isEditable: Bool

A Boolean value that controls whether the text views sharing the receiver’s layout manager allow the user to edit text.

var isRichText: Bool

A Boolean value that controls whether the text views sharing the receiver’s layout manager allow the user to apply attributes to specific ranges of text.

### Customizing subclass behaviors

func updateFontPanel()

Updates the Font panel to contain the font attributes of the selection.

func updateRuler()

Updates the ruler view in the receiver’s enclosing scroll view to reflect the selection’s paragraph and marker attributes.

var acceptableDragTypes: [NSPasteboard.PasteboardType]

The data types that the receiver accepts as the destination view of a dragging operation.

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

