

- AppKit
- NSTextField
-  init(labelWithAttributedString:) 

Initializer

# init(labelWithAttributedString:)

Creates a text field for use as a static label that displays styled text, doesn’t wrap, and doesn’t have selectable text.

macOS 10.12+

``` source
@MainActor
convenience init(labelWithAttributedString attributedStringValue: NSAttributedString)
```

## Parameters 

`attributedStringValue`  

An attributed string to use as the content of the label.

## Return Value

A text field that displays the specified attributed string as a static label.

## Discussion

The text field determines its line-break mode by inspecting the paragraph style attributes in the attributed string.

Note

When the text field has an attributed string value, the system ignores the textColor, font, alignment, lineBreakMode, and `lineBreakStrategy` properties. Set the foregroundColor, font, alignment, linebreakmode, and lineBreakStrategy properties in the attributed string instead.

## See Also

### Creating Text Fields

convenience init(labelWithString: String)

Initializes a text field for use as a static label that uses the system default font, doesn’t wrap, and doesn’t have selectable text.

convenience init(string: String)

Initializes a single-line editable text field for user input using the system default font and standard visual appearance.

convenience init(wrappingLabelWithString: String)

Initializes a text field for use as a multiline static label with selectable text that uses the system default font.

