

- AppKit
- NSApplication
-  NSApplication.PresentationOptions 

Structure

# NSApplication.PresentationOptions

Constants that control the presentation of the app, typically for fullscreen apps such as games or kiosks.

macOS 10.6+

``` source
struct PresentationOptions
```

## Overview

There are restrictions on the combination of presentation options that can be set simultaneously:

- autoHideDock and hideDock are mutually exclusive: You may specify one or the other, but not both.

- autoHideMenuBar and hideMenuBar are mutually exclusive: You may specify one or the other, but not both.

- If you specify hideMenuBar, it must be accompanied by hideDock.

- If you specify autoHideMenuBar, it must be accompanied by either hideDock or autoHideDock.

- If you specify any of disableProcessSwitching, disableForceQuit, disableSessionTermination, or disableMenuBarTransparency, it must be accompanied by either hideDock or autoHideDock.

- autoHideToolbar may be used only when both fullScreen and autoHideMenuBar are also set.

When NSApplication receives a parameter value that does not conform to these requirements, it raises an invalidArgumentException.

## Topics

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

static var disableProcessSwitching: NSApplication.PresentationOptions

The process switching user interface (Command + Tab to cycle through apps) is disabled.

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

### Initializers

init(rawValue: UInt)

Initializes a new presentation options structure.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Managing the App’s Appearance

var appearance: NSAppearance?

The appearance associated with the app’s windows.

var effectiveAppearance: NSAppearance

The appearance that AppKit uses to draw the app’s interface.

var currentSystemPresentationOptions: NSApplication.PresentationOptions

The set of app presentation options that are currently in effect for the system.

var presentationOptions: NSApplication.PresentationOptions

The presentation options that should be in effect for the system when this app is active.

