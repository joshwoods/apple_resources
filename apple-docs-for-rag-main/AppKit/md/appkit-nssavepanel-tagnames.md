

- AppKit
- NSSavePanel
-  tagNames 

Instance Property

# tagNames

The tag names that you want to include on a saved file.

macOS 10.9+

``` source
@MainActor
var tagNames: [String]? { get set }
```

## Discussion

When the value of showsTagField is true, use this property to provide an array of strings that represent the initial tag names to display in the panel. If you set the property to `nil` or an empty array, the panel displays no initial tag names.

Note

The Tags field is appropriate only in a Save panel.

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

var nameFieldStringValue: String

The user-editable filename currently shown in the name field.

var directoryURL: URL?

The current directory shown in the panel.

var accessoryView: NSView?

The custom accessory view for the current app.

var showsTagField: Bool

A Boolean value that indicates whether the panel displays the Tags field.

