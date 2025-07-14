

- AppKit
- NSPDFPanel
-  options 

Instance Property

# options

A set of configuration options that determine the accessory views the PDF panel should display.

macOS 10.9+

``` source
@MainActor
var options: NSPDFPanel.Options { get set }
```

## Discussion

You specify a set of options by combining the appropriate constants defined in NSPDFPanel.Options.

## See Also

### Managing the Contents of a PDF Panel

var accessoryController: NSViewController?

A view controller for the accessory view that the panel can present.

var defaultFileName: String

The initial value for the user-editable filename shown in the name field of the PDF panel.

