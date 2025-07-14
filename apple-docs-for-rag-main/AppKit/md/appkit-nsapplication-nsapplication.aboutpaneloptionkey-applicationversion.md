

- AppKit
- NSApplication
- NSApplication.AboutPanelOptionKey
-  applicationVersion 

Type Property

# applicationVersion

The version information to display in the About panel.

macOS 10.13+

``` source
static let applicationVersion: NSApplication.AboutPanelOptionKey
```

## Discussion

The value of this key is an NSString object with the app version (“Version 1.0”). If not specified, AppKit obtains the version string from the `CFBundleShortVersionString` key in the app’s `Info.plist` file. If neither is available, AppKit uses the build version, printed as `Version x.x`.

## See Also

### Option Keys

static let applicationIcon: NSApplication.AboutPanelOptionKey

The icon to display for the app in the About panel.

static let applicationName: NSApplication.AboutPanelOptionKey

The name of the application to display in the About panel.

static let credits: NSApplication.AboutPanelOptionKey

The credits string to display in the About panel.

static let version: NSApplication.AboutPanelOptionKey

The version number to display in the About panel.

