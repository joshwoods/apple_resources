

- AppKit
- App and Environment
- NSApplication
-  Menus 

API Collection

# Menus

Access the app’s main menu items and update the window and services menus.

## Topics

### Accessing the Main Menu

var mainMenu: NSMenu?

The app’s main menu bar.

var isAutomaticCustomizeTouchBarMenuItemEnabled: Bool

A Boolean value indicating whether the main menu contains an item for customizing the contents of the Touch Bar.

### Managing the Window Menu

var windowsMenu: NSMenu?

The Window menu of the app.

func addWindowsItem(NSWindow, title: String, filename: Bool)

Adds an item to the Window menu for a given window.

func changeWindowsItem(NSWindow, title: String, filename: Bool)

Changes the item for a given window in the Window menu to a given string.

func removeWindowsItem(NSWindow)

Removes the Window menu item for a given window.

func updateWindowsItem(NSWindow)

Updates the Window menu item for a given window to reflect the edited status of that window.

### Managing the Services Menu

func registerServicesMenuSendTypes([NSPasteboard.PasteboardType], returnTypes: [NSPasteboard.PasteboardType])

Registers the pasteboard types the receiver can send and receive in response to service requests.

var servicesMenu: NSMenu?

The app’s Services menu.

## See Also

### Managing Windows, Panels, and Menus

App Windows

Show, hide, minimize, arrange, and update your app’s windows.

Modal Windows and Panels

Display a modal window or show one of the standard app panels, such as the app’s About panel.

