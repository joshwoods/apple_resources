

- AppKit
- NSTextView
-  outline(\_:) 

Instance Method

# outline(\_:)

Adds the outline attribute to the selected text attributes if absent; removes the attribute if present.

macOS

``` source
@MainActor
func outline(_ sender: Any?)
```

## Parameters 

`sender`  

The control that sent the message; may be `nil`.

## Discussion

If there is a selection and the first character of the selected range has a non-zero stroke width, or if there is no selection and the typing attributes have a non-zero stroke width, then the stroke width is removed; otherwise the value of `NSStrokeWidthAttributeName` is set to the default value for outline (3.0).

Operates on the selected range if the receiver contains rich text. For plain text the range is the entire contents of the receiver.

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

func setBaseWritingDirection(NSWritingDirection, range: NSRange)

Sets the base writing direction of a range of text.

var defaultParagraphStyle: NSParagraphStyle?

The receiver’s default paragraph style.

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

