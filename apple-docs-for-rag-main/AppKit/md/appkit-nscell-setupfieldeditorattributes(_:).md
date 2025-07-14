

- AppKit
- NSCell
-  setUpFieldEditorAttributes(\_:) 

Instance Method

# setUpFieldEditorAttributes(\_:)

Configures the textual and background attributes of the receiver’s field editor.

macOS

``` source
@MainActor
func setUpFieldEditorAttributes(_ textObj: NSText) -> NSText
```

## Parameters 

`textObj`  

The field editor to configure. .

## Return Value

The configured field editor.

## Discussion

If the receiver is disabled, this method sets the text color to dark gray; otherwise the method sets it to the default color. If the receiver has a bezeled border, this method sets the background to the default color for text backgrounds; otherwise, the method sets it to the color of the receiver’s `NSControl` object.

You should not use this method to substitute a new field editor. setUpFieldEditorAttributes(_:) is intended to modify the attributes of the text object (that is, the field editor) passed into it and return that text object. If you want to substitute your own field editor, use the fieldEditor(_:for:) method or the windowWillReturnFieldEditor(_:to:) delegate method of `NSWindow`.

## See Also

### Modifying Textual Attributes

var isEditable: Bool

A Boolean value indicating whether the cell is editable.

var isSelectable: Bool

A Boolean value indicating whether the cell’s text can be selected.

var isScrollable: Bool

A Boolean value indicating whether excess text scrolls past the cell’s bounds.

var alignment: NSTextAlignment

The alignment of the cell’s text.

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

var title: String

The cell’s title text.

