

- AppKit
- NSPrintPanel
- NSPrintPanel.Options
-  showsPageSetupAccessory 

Type Property

# showsPageSetupAccessory

The Print panel includes a separate accessory view for manipulating the paper size, orientation, and scaling attributes.

macOS 10.5+

``` source
static var showsPageSetupAccessory: NSPrintPanel.Options { get }
```

## Discussion

Page setup fields that are already configured for display on the main portion of the Print panel appear there and not on this accessory panel.

## See Also

### Constants

static var showsCopies: NSPrintPanel.Options

The Print panel includes a field for manipulating the number of copies being printed.

static var showsPageRange: NSPrintPanel.Options

The Print panel includes a set of fields for manipulating the range of pages being printed.

static var showsPaperSize: NSPrintPanel.Options

The Print panel includes a control for manipulating the paper size of the printer.

static var showsOrientation: NSPrintPanel.Options

The Print panel includes a control for manipulating the page orientation.

static var showsScaling: NSPrintPanel.Options

The Print panel includes a control for scaling the printed output.

static var showsPrintSelection: NSPrintPanel.Options

The Print panel includes an additional selection option for paper range.

static var showsPreview: NSPrintPanel.Options

The Print panel displays a built-in preview of the document contents.

