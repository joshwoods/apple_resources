

- AppKit
- NSSavePanel
-  accessoryView 

Instance Property

# accessoryView

The custom accessory view for the current app.

macOS

``` source
@MainActor
var accessoryView: NSView? { get set }
```

## Discussion

You can customize the panel by adding a custom view. The custom object you add appears just above the OK and Cancel buttons at the bottom of the panel. The `NSSavePanel` object automatically resizes itself to accommodate `accessoryView`. Use this property to change the accessory view as needed. If `accessoryView` is `nil`, the Save panel removes the current accessory view.

The panel relinquishes ownership of the accessory view after the panel is closed. If you want to reuse the accessory view, don’t rely on the panel to hold onto the accessory view until the next time you use it; instead, maintain your own strong reference to the view.

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

var showsTagField: Bool

A Boolean value that indicates whether the panel displays the Tags field.

var tagNames: [String]?

The tag names that you want to include on a saved file.

