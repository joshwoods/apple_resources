

- AppKit
- NSTextInsertionIndicator
-  automaticModeOptions 

Instance Property

# automaticModeOptions

Options that affect the automatic display mode.

macOS 14.0+

``` source
@MainActor
var automaticModeOptions: NSTextInsertionIndicator.AutomaticModeOptions { get set }
```

## Mentioned in 

Adopting the system text cursor in custom text views

## Discussion

Defaults to showEffectsView.

## See Also

### Setting the display mode

var displayMode: NSTextInsertionIndicator.DisplayMode

A value that describes the display mode of an indicator.

struct AutomaticModeOptions

Options that affect the automatic display mode.

enum DisplayMode

Constants that determine how to display the system text cursor in a custom text UI.

