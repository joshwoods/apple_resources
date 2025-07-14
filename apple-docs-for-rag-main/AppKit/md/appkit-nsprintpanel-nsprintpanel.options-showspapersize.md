

- AppKit
- NSPrintPanel
- NSPrintPanel.Options
-  showsPaperSize 

Type Property

# showsPaperSize

The Print panel includes a control for manipulating the paper size of the printer.

macOS 10.5+

``` source
static var showsPaperSize: NSPrintPanel.Options { get }
```

## Discussion

This control is separate from any accessory views.

## See Also

### Constants

static var showsCopies: NSPrintPanel.Options

The Print panel includes a field for manipulating the number of copies being printed.

static var showsPageRange: NSPrintPanel.Options

The Print panel includes a set of fields for manipulating the range of pages being printed.

static var showsOrientation: NSPrintPanel.Options

The Print panel includes a control for manipulating the page orientation.

static var showsScaling: NSPrintPanel.Options

The Print panel includes a control for scaling the printed output.

static var showsPrintSelection: NSPrintPanel.Options

The Print panel includes an additional selection option for paper range.

static var showsPageSetupAccessory: NSPrintPanel.Options

The Print panel includes a separate accessory view for manipulating the paper size, orientation, and scaling attributes.

static var showsPreview: NSPrintPanel.Options

The Print panel displays a built-in preview of the document contents.

