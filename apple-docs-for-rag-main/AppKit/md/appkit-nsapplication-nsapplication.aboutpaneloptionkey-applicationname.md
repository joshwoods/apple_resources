

- AppKit
- NSApplication
- NSApplication.AboutPanelOptionKey
-  applicationName 

Type Property

# applicationName

The name of the application to display in the About panel.

macOS 10.13+

``` source
static let applicationName: NSApplication.AboutPanelOptionKey
```

## Discussion

The value of this key is an NSString object containing the app’s name. If you do not specify this key, AppKit uses the value of the `CFBundleName` key from the app’s `Info.plist` file. If neither is found, AppKit uses the name of the app’s process.

## See Also

### Option Keys

static let applicationIcon: NSApplication.AboutPanelOptionKey

The icon to display for the app in the About panel.

static let applicationVersion: NSApplication.AboutPanelOptionKey

The version information to display in the About panel.

static let credits: NSApplication.AboutPanelOptionKey

The credits string to display in the About panel.

static let version: NSApplication.AboutPanelOptionKey

The version number to display in the About panel.

