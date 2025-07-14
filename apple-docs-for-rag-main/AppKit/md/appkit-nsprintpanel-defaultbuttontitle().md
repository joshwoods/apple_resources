

- AppKit
- NSPrintPanel
-  defaultButtonTitle() 

Instance Method

# defaultButtonTitle()

Returns the title of the Print panel’s default button.

macOS 10.5+

``` source
@MainActor
func defaultButtonTitle() -> String?
```

## Return Value

The title of the default button.

## See Also

### Customizing the Panel

var jobStyleHint: NSPrintPanel.JobStyleHint?

The type of settings that the print panel displays.

struct JobStyleHint

Constants that specify job style hints for activating the simplified Print panel interface and setting the options to display.

var options: NSPrintPanel.Options

The current configuration options for the Print panel.

struct Options

Constants that specify options for configuring the contents of the main Print panel.

func setDefaultButtonTitle(String?)

Sets the title of the Print panel’s default button.

var helpAnchor: NSHelpManager.AnchorName?

The HTML help anchor associated with the Print panel.

