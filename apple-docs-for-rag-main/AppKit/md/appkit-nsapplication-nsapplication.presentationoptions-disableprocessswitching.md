

- AppKit
- NSApplication
- NSApplication.PresentationOptions
-  disableProcessSwitching 

Type Property

# disableProcessSwitching

The process switching user interface (Command + Tab to cycle through apps) is disabled.

macOS 10.6+

``` source
static var disableProcessSwitching: NSApplication.PresentationOptions { get }
```

## See Also

### Presentation Options

static var autoHideDock: NSApplication.PresentationOptions

The dock is normally hidden, but automatically appears when moused near.

static var hideDock: NSApplication.PresentationOptions

The dock is entirely hidden and disabled.

static var autoHideMenuBar: NSApplication.PresentationOptions

The menu bar is normally hidden, but automatically appears when moused near.

static var hideMenuBar: NSApplication.PresentationOptions

The menu bar is entirely hidden and disabled.

static var disableAppleMenu: NSApplication.PresentationOptions

All Apple Menu items are disabled.

static var disableForceQuit: NSApplication.PresentationOptions

The force quit panel (displayed by pressing Command + Option + Esc) is disabled

static var disableSessionTermination: NSApplication.PresentationOptions

The panel that shows the Restart, Shut Down, and Log Out options that are displayed as a result of pushing the power key is disabled.

static var disableHideApplication: NSApplication.PresentationOptions

The app’s “Hide” menu item is disabled.

static var disableMenuBarTransparency: NSApplication.PresentationOptions

The menu bar transparency appearance is disabled.

static var fullScreen: NSApplication.PresentationOptions

The app is in fullscreen mode.

static var autoHideToolbar: NSApplication.PresentationOptions

When in fullscreen mode the window toolbar is detached from window and hides and shows with autoHidden menuBar.

static var disableCursorLocationAssistance: NSApplication.PresentationOptions

The behavior that allows the user to shake the mouse to locate the cursor is disabled.

