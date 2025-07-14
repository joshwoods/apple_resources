

- AppKit
- NSPrintPanel
-  helpAnchor 

Instance Property

# helpAnchor

The HTML help anchor associated with the Print panel.

macOS 10.5+

``` source
@MainActor
var helpAnchor: NSHelpManager.AnchorName? { get set }
```

## Discussion

Use this property to specify the anchor name in your Apple Help file. The string you assign should contain only the name portion of the HTML anchor element.

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

func defaultButtonTitle() -> String?

Returns the title of the Print panel’s default button.

func setDefaultButtonTitle(String?)

Sets the title of the Print panel’s default button.

