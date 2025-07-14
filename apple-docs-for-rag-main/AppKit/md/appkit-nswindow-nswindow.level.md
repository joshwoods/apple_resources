

- AppKit
- NSWindow
-  NSWindow.Level 

Structure

# NSWindow.Level

The standard window levels in macOS.

macOS

``` source
struct Level
```

## Discussion

The stacking of levels takes precedence over the stacking of windows within each level. That is, even the bottom window in a level will obscure the top window of the next level down. Levels are listed in order from lowest to highest. These constants are mapped (using `#define` statements) to corresponding elements in CGWindowLevelKey.

## Topics

### Constants

static let dock: NSWindow.Level

The level for the dock.

Deprecated

static let floating: NSWindow.Level

Useful for floating palettes.

static let mainMenu: NSWindow.Level

Reserved for the application’s main menu.

static let modalPanel: NSWindow.Level

The level for a modal panel.

static let normal: NSWindow.Level

The default level for `NSWindow` objects.

static let popUpMenu: NSWindow.Level

The level for a pop-up menu.

static let screenSaver: NSWindow.Level

The level for a screen saver.

static let statusBar: NSWindow.Level

The level for a status window.

static let submenu: NSWindow.Level

Reserved for submenus. Synonymous with `NSTornOffMenuWindowLevel`, which is preferred.

static let tornOffMenu: NSWindow.Level

The level for a torn-off menu. Synonymous with `NSSubmenuWindowLevel`.

### Creating a Window Level

init(Int)

Creates a window level using the given integer value.

init(rawValue: Int)

Creates a window level using the given raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Comparable
- Copyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing Window Layers

func orderOut(Any?)

Removes the window from the screen list, which hides the window.

func orderBack(Any?)

Moves the window to the back of its level in the screen list, without changing either the key window or the main window.

func orderFront(Any?)

Moves the window to the front of its level in the screen list, without changing either the key window or the main window.

func orderFrontRegardless()

Moves the window to the front of its level, even if its application isn’t active, without changing either the key window or the main window.

func order(NSWindow.OrderingMode, relativeTo: Int)

Repositions the window’s window device in the window server’s screen list.

var level: NSWindow.Level

The window level of the window.

