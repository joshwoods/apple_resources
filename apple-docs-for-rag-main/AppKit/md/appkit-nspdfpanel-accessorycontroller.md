

- AppKit
- NSPDFPanel
-  accessoryController 

Instance Property

# accessoryController

A view controller for the accessory view that the panel can present.

macOS 10.9+

``` source
@MainActor
var accessoryController: NSViewController? { get set }
```

## Discussion

The PDF panel passes an NSPDFInfo object to the accessory view controller to display the various attributes associated with the PDF file. Unlike a print panel (that is, an NSPrintPanel object), a PDF panel can have only one accessory view.

## See Also

### Managing the Contents of a PDF Panel

var options: NSPDFPanel.Options

A set of configuration options that determine the accessory views the PDF panel should display.

var defaultFileName: String

The initial value for the user-editable filename shown in the name field of the PDF panel.

