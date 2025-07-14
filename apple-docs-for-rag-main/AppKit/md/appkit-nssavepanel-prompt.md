

- AppKit
- NSSavePanel
-  prompt 

Instance Property

# prompt

The text to display in the default button.

macOS

``` source
@MainActor
var prompt: String! { get set }
```

## Discussion

The prompt appears on all NSSavePanel objects (or all NSOpenPanel objects if this property is on an NSOpenPanel instance) in your application. By default, the text in the default button is “Open” for an Open panel and “Save” for a Save panel.

Use short words or phrases, such as “Open,” “Save,” “Set,” or “Choose,” on the button. The button is not resized to accommodate long prompts.

## See Also

### Configuring the Panel’s Appearance

var title: String!

The title of the panel.

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

