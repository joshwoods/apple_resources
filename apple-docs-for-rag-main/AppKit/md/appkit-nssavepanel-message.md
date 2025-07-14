

- AppKit
- NSSavePanel
-  message 

Instance Property

# message

The message text displayed in the panel.

macOS

``` source
@MainActor
var message: String! { get set }
```

## Discussion

This prompt appears on all NSSavePanel objects (or all NSOpenPanel objects if this property is on an NSOpenPanel instance) in your application. The default message text is an empty string.

## See Also

### Configuring the Panel’s Appearance

var title: String!

The title of the panel.

var prompt: String!

The text to display in the default button.

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

