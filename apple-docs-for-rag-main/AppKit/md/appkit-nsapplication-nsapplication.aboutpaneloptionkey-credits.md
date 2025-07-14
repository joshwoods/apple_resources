

- AppKit
- NSApplication
- NSApplication.AboutPanelOptionKey
-  credits 

Type Property

# credits

The credits string to display in the About panel.

macOS 10.13+

``` source
static let credits: NSApplication.AboutPanelOptionKey
```

## Discussion

The value of this key is an NSAttributedString displayed in the info area of the panel. If not specified, AppKit then looks for a file named “Credits.html”, “Credits.rtf”, and “Credits.rtfd”, in that order, in the bundle returned by the Bundle class method main. The first file found is used. If none is found, the info area is left blank.

## See Also

### Option Keys

static let applicationIcon: NSApplication.AboutPanelOptionKey

The icon to display for the app in the About panel.

static let applicationName: NSApplication.AboutPanelOptionKey

The name of the application to display in the About panel.

static let applicationVersion: NSApplication.AboutPanelOptionKey

The version information to display in the About panel.

static let version: NSApplication.AboutPanelOptionKey

The version number to display in the About panel.

