

- AppKit
- NSPrintPanel
-  NSPrintPanel.Options 

Structure

# NSPrintPanel.Options

Constants that specify options for configuring the contents of the main Print panel.

macOS 10.5+

``` source
struct Options
```

## Topics

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

static var showsPageSetupAccessory: NSPrintPanel.Options

The Print panel includes a separate accessory view for manipulating the paper size, orientation, and scaling attributes.

static var showsPreview: NSPrintPanel.Options

The Print panel displays a built-in preview of the document contents.

### Initializers

init(rawValue: UInt)

Creates a new instance with the specified raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Customizing the Panel

var jobStyleHint: NSPrintPanel.JobStyleHint?

The type of settings that the print panel displays.

struct JobStyleHint

Constants that specify job style hints for activating the simplified Print panel interface and setting the options to display.

var options: NSPrintPanel.Options

The current configuration options for the Print panel.

func defaultButtonTitle() -> String?

Returns the title of the Print panel’s default button.

func setDefaultButtonTitle(String?)

Sets the title of the Print panel’s default button.

var helpAnchor: NSHelpManager.AnchorName?

The HTML help anchor associated with the Print panel.

