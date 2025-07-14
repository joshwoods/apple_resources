

- AppKit
- NSPrintPanel
-  NSPrintPanel.JobStyleHint 

Structure

# NSPrintPanel.JobStyleHint

Constants that specify job style hints for activating the simplified Print panel interface and setting the options to display.

macOS

``` source
struct JobStyleHint
```

## Topics

### Constants

static let photo: NSPrintPanel.JobStyleHint

Output contains photographic data.

static let allPresets: NSPrintPanel.JobStyleHint

Output appropriate to all graphics types.

static let noPresets: NSPrintPanel.JobStyleHint

Output excludes all graphics printing.

### Initializers

init(rawValue: String)

Creates a new instance with the specified raw value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Customizing the Panel

var jobStyleHint: NSPrintPanel.JobStyleHint?

The type of settings that the print panel displays.

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

