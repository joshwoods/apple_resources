

- AppKit
- NSPDFPanel
-  defaultFileName 

Instance Property

# defaultFileName

The initial value for the user-editable filename shown in the name field of the PDF panel.

macOS 10.9+

``` source
@MainActor
var defaultFileName: String { get set }
```

## Discussion

The `defaultFileName` string should never include a file extension. By default, the string’s value is “Untitled” (or its equivalent for the current locale).

## See Also

### Managing the Contents of a PDF Panel

var accessoryController: NSViewController?

A view controller for the accessory view that the panel can present.

var options: NSPDFPanel.Options

A set of configuration options that determine the accessory views the PDF panel should display.

