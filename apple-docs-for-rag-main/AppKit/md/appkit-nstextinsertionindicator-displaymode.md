

- AppKit
- NSTextInsertionIndicator
-  displayMode 

Instance Property

# displayMode

A value that describes the display mode of an indicator.

macOS 14.0+

``` source
@MainActor
var displayMode: NSTextInsertionIndicator.DisplayMode { get set }
```

## Discussion

Set the displayMode to NSTextInsertionIndicator.DisplayMode.automatic when your custom view becomes the first responder. When your custom view resigns first responder, set the displayMode to NSTextInsertionIndicator.DisplayMode.hidden to indicate that key events aren’t sent to your view.

## See Also

### Setting the display mode

var automaticModeOptions: NSTextInsertionIndicator.AutomaticModeOptions

Options that affect the automatic display mode.

struct AutomaticModeOptions

Options that affect the automatic display mode.

enum DisplayMode

Constants that determine how to display the system text cursor in a custom text UI.

