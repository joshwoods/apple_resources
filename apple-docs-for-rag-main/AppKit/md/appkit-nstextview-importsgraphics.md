

- AppKit
- NSTextView
-  importsGraphics 

Instance Property

# importsGraphics

A Boolean value that controls whether the text views sharing the receiver’s layout manager allow the user to import files by dragging.

macOS

``` source
@MainActor
var importsGraphics: Bool { get set }
```

## Discussion

true to allow the user to import files by dragging onto the text views sharing the receiver’s layout manager, false otherwise.

Text views that are set to accept dragged files are also set to allow rich text. By default, text views don’t accept dragged files but do allow rich text.

## See Also

### Related Documentation

func insert(NSAttributedString, at: Int)

Inserts the characters and attributes of the given attributed string into the receiver at the given index.

init(attachment: NSTextAttachment)

Creates an attributed string with an attachment.

var textStorage: NSTextStorage?

The receiver’s text storage object.

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

func setBaseWritingDirection(NSWritingDirection, range: NSRange)

Sets the base writing direction of a range of text.

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

