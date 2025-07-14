

- AppKit
- NSPrintPanel
-  setDefaultButtonTitle(\_:) 

Instance Method

# setDefaultButtonTitle(\_:)

Sets the title of the Print panel’s default button.

macOS 10.5+

``` source
@MainActor
func setDefaultButtonTitle(_ defaultButtonTitle: String?)
```

## Parameters 

`defaultButtonTitle`  

The string to use for the button title.

## Discussion

You can use this method to change the default button title from “Print” to something more appropriate for your usage of the panel. For example, if you are using the Print panel to save a representation of the document to a file, you might change the title to “Save”.

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

var helpAnchor: NSHelpManager.AnchorName?

The HTML help anchor associated with the Print panel.

