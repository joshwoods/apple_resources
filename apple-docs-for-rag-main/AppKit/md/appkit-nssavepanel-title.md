

- AppKit
- NSSavePanel
-  title 

Instance Property

# title

The title of the panel.

macOS

``` source
@MainActor
var title: String! { get set }
```

## Discussion

By default, “Save” is the title string. If you adapt the `NSSavePanel` object for other uses, its title should reflect the user action that brings it to the screen.

## See Also

### Configuring the Panel’s Appearance

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

var tagNames: [String]?

The tag names that you want to include on a saved file.

