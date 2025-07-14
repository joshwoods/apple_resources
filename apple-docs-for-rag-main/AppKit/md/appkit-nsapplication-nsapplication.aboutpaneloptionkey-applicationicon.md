

- AppKit
- NSApplication
- NSApplication.AboutPanelOptionKey
-  applicationIcon 

Type Property

# applicationIcon

The icon to display for the app in the About panel.

macOS 10.13+

``` source
static let applicationIcon: NSApplication.AboutPanelOptionKey
```

## Discussion

The value associated with this key is an NSImage object. If you do not specify an image, AppKit looks for an image with the name `NSApplicationIcon`. If neither is available, this method uses the generic app icon.

## See Also

### Option Keys

static let applicationName: NSApplication.AboutPanelOptionKey

The name of the application to display in the About panel.

static let applicationVersion: NSApplication.AboutPanelOptionKey

The version information to display in the About panel.

static let credits: NSApplication.AboutPanelOptionKey

The credits string to display in the About panel.

static let version: NSApplication.AboutPanelOptionKey

The version number to display in the About panel.

