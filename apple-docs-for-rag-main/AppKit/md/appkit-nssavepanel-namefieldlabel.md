

- AppKit
- NSSavePanel
-  nameFieldLabel 

Instance Property

# nameFieldLabel

The label text displayed in front of the filename text field.

macOS

``` source
@MainActor
var nameFieldLabel: String! { get set }
```

## Discussion

The default value of this property is “Save As:”.

## See Also

### Configuring the Panel’s Appearance

var title: String!

The title of the panel.

var prompt: String!

The text to display in the default button.

var message: String!

The message text displayed in the panel.

var nameFieldStringValue: String

The user-editable filename currently shown in the name field.

var directoryURL: URL?

The current directory shown in the panel.

var accessoryView: NSView?

The custom accessory view for the current app.

var showsTagField: Bool

A Boolean value that indicates whether the panel displays the Tags field.

var tagNames: [String]?

The tag names that you want to include on a saved file.

