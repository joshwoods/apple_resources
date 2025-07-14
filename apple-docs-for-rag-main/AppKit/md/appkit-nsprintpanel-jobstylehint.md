

- AppKit
- NSPrintPanel
-  jobStyleHint 

Instance Property

# jobStyleHint

The type of settings that the print panel displays.

macOS

``` source
@MainActor
var jobStyleHint: NSPrintPanel.JobStyleHint? { get set }
```

## Discussion

This property controls the set of items that appear in the Presets menu of the simplified Print panel interface. For a list of supported job style hints, see `Job Style Hints`. Set this property to `nil` to deactivate the simplified Print panel interface and use the standard interface instead (the equivalent of Core Printing’s `kPMPresetGraphicsTypeGeneral`).

## See Also

### Customizing the Panel

struct JobStyleHint

Constants that specify job style hints for activating the simplified Print panel interface and setting the options to display.

var options: NSPrintPanel.Options

The current configuration options for the Print panel.

struct Options

Constants that specify options for configuring the contents of the main Print panel.

func defaultButtonTitle() -> String?

Returns the title of the Print panel’s default button.

func setDefaultButtonTitle(String?)

Sets the title of the Print panel’s default button.

var helpAnchor: NSHelpManager.AnchorName?

The HTML help anchor associated with the Print panel.

