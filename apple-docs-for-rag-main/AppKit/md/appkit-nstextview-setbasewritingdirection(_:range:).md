

- AppKit
- NSTextView
-  setBaseWritingDirection(\_:range:) 

Instance Method

# setBaseWritingDirection(\_:range:)

Sets the base writing direction of a range of text.

macOS

``` source
@MainActor
func setBaseWritingDirection(
    _ writingDirection: NSWritingDirection,
    range: NSRange
)
```

## Parameters 

`writingDirection`  

The new writing direction for the text in `range`.

`range`  

The range of text that will have the new writing direction.

## Discussion

Invoke this method to change the base writing direction from left-to-right to right-to-left for languages like Hebrew and Arabic, for example.

This method does not include undo support by default. Clients must invoke shouldChangeText(inRanges:replacementStrings:) or shouldChangeText(in:replacementString:) to include this method in an undoable action.

## See Also

### Setting behavioral attributes

var allowsUndo: Bool

A Boolean value that indicates whether the receiver allows undo.

var isEditable: Bool

A Boolean value that controls whether the text views sharing the receiver’s layout manager allow the user to edit text.

var isSelectable: Bool

A Boolean value that controls whether the text views sharing the receiver’s layout manager allow the user to select text.

var isFieldEditor: Bool

A Boolean value that controls whether the text views sharing the receiver’s layout manager behave as field editors.

var isRichText: Bool

A Boolean value that controls whether the text views sharing the receiver’s layout manager allow the user to apply attributes to specific ranges of text.

var importsGraphics: Bool

A Boolean value that controls whether the text views sharing the receiver’s layout manager allow the user to import files by dragging.

var defaultParagraphStyle: NSParagraphStyle?

The receiver’s default paragraph style.

func outline(Any?)

Adds the outline attribute to the selected text attributes if absent; removes the attribute if present.

var allowsImageEditing: Bool

Indicates whether image attachments should permit editing of their images.

var isAutomaticQuoteSubstitutionEnabled: Bool

A Boolean value that enables and disables automatic quotation mark substitution.

func toggleAutomaticQuoteSubstitution(Any?)

Changes the state of automatic quotation mark substitution from enabled to disabled and vice versa.

var isAutomaticLinkDetectionEnabled: Bool

A Boolean value that enables or disables automatic link detection.

func toggleAutomaticLinkDetection(Any?)

Changes the state of automatic link detection from enabled to disabled and vice versa.

var displaysLinkToolTips: Bool

A Boolean value that indicates whether the text view automatically supplies the destination of a link as a tooltip for text that has a link attribute.

var isAutomaticTextCompletionEnabled: Bool

A Boolean value that indicates whether the text view supplies autocompletion suggestions as the user types.

