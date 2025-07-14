

- AppKit
- NSTextField
-  init(wrappingLabelWithString:) 

Initializer

# init(wrappingLabelWithString:)

Initializes a text field for use as a multiline static label with selectable text that uses the system default font.

macOS 10.12+

``` source
@MainActor
convenience init(wrappingLabelWithString stringValue: String)
```

## Parameters 

`stringValue`  

A string to use as the initial content of the editable text field.

## Return Value

A multiline text field that displays the specified string.

## See Also

### Creating Text Fields

convenience init(labelWithAttributedString: NSAttributedString)

Creates a text field for use as a static label that displays styled text, doesn’t wrap, and doesn’t have selectable text.

convenience init(labelWithString: String)

Initializes a text field for use as a static label that uses the system default font, doesn’t wrap, and doesn’t have selectable text.

convenience init(string: String)

Initializes a single-line editable text field for user input using the system default font and standard visual appearance.

