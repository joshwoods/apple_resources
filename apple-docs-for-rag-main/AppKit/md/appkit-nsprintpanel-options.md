

- AppKit
- NSPrintPanel
-  options 

Instance Property

# options

The current configuration options for the Print panel.

macOS 10.5+

``` source
@MainActor
var options: NSPrintPanel.Options { get set }
```

## Discussion

You can specify multiple options by adding them together. For a list of supported options, see NSPrintPanel.Options.

## See Also

### Customizing the Panel

var jobStyleHint: NSPrintPanel.JobStyleHint?

The type of settings that the print panel displays.

struct JobStyleHint

Constants that specify job style hints for activating the simplified Print panel interface and setting the options to display.

struct Options

Constants that specify options for configuring the contents of the main Print panel.

func defaultButtonTitle() -> String?

Returns the title of the Print panel’s default button.

func setDefaultButtonTitle(String?)

Sets the title of the Print panel’s default button.

var helpAnchor: NSHelpManager.AnchorName?

The HTML help anchor associated with the Print panel.

