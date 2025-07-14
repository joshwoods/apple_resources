

- AppKit
- NSApplication
-  NSApplication.AboutPanelOptionKey 

Structure

# NSApplication.AboutPanelOptionKey

Keys to include in the options dictionary when displaying an About panel.

macOS

``` source
struct AboutPanelOptionKey
```

## Topics

### Option Keys

static let applicationIcon: NSApplication.AboutPanelOptionKey

The icon to display for the app in the About panel.

static let applicationName: NSApplication.AboutPanelOptionKey

The name of the application to display in the About panel.

static let applicationVersion: NSApplication.AboutPanelOptionKey

The version information to display in the About panel.

static let credits: NSApplication.AboutPanelOptionKey

The credits string to display in the About panel.

static let version: NSApplication.AboutPanelOptionKey

The version number to display in the About panel.

### Initializers

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing Panels

func orderFrontColorPanel(Any?)

Brings up the color panel, an instance of `NSColorPanel`.

func orderFrontStandardAboutPanel(Any?)

Displays a standard About window.

func orderFrontStandardAboutPanel(options: [NSApplication.AboutPanelOptionKey : Any])

Displays a standard About window with information from a given options dictionary.

func orderFrontCharacterPalette(Any?)

Opens the character palette.

func runPageLayout(Any?)

Displays the receiver’s page layout panel, an instance of `NSPageLayout`.

