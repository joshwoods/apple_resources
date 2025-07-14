

- AppKit
- NSCell
-  alignment 

Instance Property

# alignment

The alignment of the cell’s text.

macOS

``` source
@MainActor
var alignment: NSTextAlignment { get set }
```

## Discussion

The default value of this property is `NSNaturalTextAlignment`. For a list of possible text alignments, see NSTextAlignment.

## See Also

### Modifying Textual Attributes

var isEditable: Bool

A Boolean value indicating whether the cell is editable.

var isSelectable: Bool

A Boolean value indicating whether the cell’s text can be selected.

var isScrollable: Bool

A Boolean value indicating whether excess text scrolls past the cell’s bounds.

var font: NSFont?

The font that the cell uses to display text.

var lineBreakMode: NSLineBreakMode

The line break mode to use when drawing text in the cell.

var truncatesLastVisibleLine: Bool

A Boolean value indicating whether the cell truncates text that does not fit within the cell’s bounds.

var wraps: Bool

A Boolean value indicating whether the cell wraps text whose length that exceeds the cell’s frame.

var baseWritingDirection: NSWritingDirection

The initial writing direction used to determine the actual writing direction for text.

var attributedStringValue: NSAttributedString

The cell’s value as an attributed string.

var allowsEditingTextAttributes: Bool

A Boolean value indicating whether the cell allows the editing of its content’s text attributes by the user.

var importsGraphics: Bool

A Boolean value indicating whether the cell supports the importation of images into its text.

func setUpFieldEditorAttributes(NSText) -> NSText

Configures the textual and background attributes of the receiver’s field editor.

var title: String

The cell’s title text.

