

- AppKit
- NSApplication
- NSApplication.AboutPanelOptionKey
-  version 

Type Property

# version

The version number to display in the About panel.

macOS 10.13+

``` source
static let version: NSApplication.AboutPanelOptionKey
```

## Discussion

The value of this key is an NSString object with the build version number of the app, such as `58.4`. AppKit displays this string as `(v58.4)`. If not specified, AppKit obtains the version number from the CFBundleVersion key of the app’s Info.plist file. If no version information is found, AppKit does not display version information.

## See Also

### Option Keys

static let applicationIcon: NSApplication.AboutPanelOptionKey

The icon to display for the app in the About panel.

static let applicationName: NSApplication.AboutPanelOptionKey

The name of the application to display in the About panel.

static let applicationVersion: NSApplication.AboutPanelOptionKey

The version information to display in the About panel.

static let credits: NSApplication.AboutPanelOptionKey

The credits string to display in the About panel.

