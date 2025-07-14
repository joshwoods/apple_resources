

- AppKit
- NSSavePanel
-  showsTagField 

Instance Property

# showsTagField

A Boolean value that indicates whether the panel displays the Tags field.

macOS 10.9+

``` source
@MainActor
var showsTagField: Bool { get set }
```

## Discussion

When the value of this property is true, the panel displays the Tags field; if false, the panel doesn’t display the Tags field. The default value is true. (Note that the Tags field is appropriate only in a Save panel.)

If you set this property to true, you are responsible for setting tag names on the resulting file after saving is complete. If you don’t set this property, macOS will automatically show the tag field and attempt to apply the tags to the file. To set tags on files, use the tagNamesKey.

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

var tagNames: [String]?

The tag names that you want to include on a saved file.

