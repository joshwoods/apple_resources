

- AppKit
- NSTextView
-  toggleAutomaticLinkDetection(\_:) 

Instance Method

# toggleAutomaticLinkDetection(\_:)

Changes the state of automatic link detection from enabled to disabled and vice versa.

macOS 10.5+

``` source
@MainActor
func toggleAutomaticLinkDetection(_ sender: Any?)
```

## Parameters 

`sender`  

The control sending the message; may be `nil`.

## Discussion

Automatic link detection causes strings representing URLs typed in the view to be automatically made into links to those URLs.

## See Also

### Related Documentation

func url(at: Int, effectiveRange: NSRangePointer) -> URL?

Returns a URL, either from a link attribute or from text at the specified location that appears to be a URL string, for use in automatic link detection.

Deprecated

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

var displaysLinkToolTips: Bool

A Boolean value that indicates whether the text view automatically supplies the destination of a link as a tooltip for text that has a link attribute.

var isAutomaticTextCompletionEnabled: Bool

A Boolean value that indicates whether the text view supplies autocompletion suggestions as the user types.

