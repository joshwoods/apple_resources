

- AppKit
- NSSavePanel
-  nameFieldStringValue 

Instance Property

# nameFieldStringValue

The user-editable filename currently shown in the name field.

macOS 10.6+

``` source
@MainActor
var nameFieldStringValue: String { get set }
```

## Discussion

The value of this property must not be `nil`. Note that the filename may not display an extension if the value of isExtensionHidden is true.

## See Also

### Configuring the Panel’s Appearance

var title: String!

The title of the panel.

var prompt: String!

The text to display in the default button.

var message: String!

The message text displayed in the panel.

var nameFieldLabel: String!

The label text displayed in front of the filename text field.

var directoryURL: URL?

The current directory shown in the panel.

var accessoryView: NSView?

The custom accessory view for the current app.

var showsTagField: Bool

A Boolean value that indicates whether the panel displays the Tags field.

var tagNames: [String]?

The tag names that you want to include on a saved file.

