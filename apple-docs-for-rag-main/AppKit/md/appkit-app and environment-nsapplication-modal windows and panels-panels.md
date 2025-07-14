

- AppKit
- App and Environment
- NSApplication
-  Modal Windows and Panels 

API Collection

# Modal Windows and Panels

Display a modal window or show one of the standard app panels, such as the app’s About panel.

## Topics

### Running a Modal Window

func runModal(for: NSWindow) -> NSApplication.ModalResponse

Starts a modal event loop for the specified window.

func stopModal()

Stops a modal event loop.

func stopModal(withCode: NSApplication.ModalResponse)

Stops a modal event loop, allowing you to return a custom result code.

func abortModal()

Aborts the event loop started by runModal(for:) or runModalSession(_:).

func beginModalSession(for: NSWindow) -> NSApplication.ModalSession

Sets up a modal session with the given window and returns a pointer to the `NSModalSession` structure representing the session.

func runModalSession(NSApplication.ModalSession) -> NSApplication.ModalResponse

Runs a given modal session, as defined in a previous invocation of beginModalSession(for:).

var modalWindow: NSWindow?

The modal window displayed by the app.

struct ModalResponse

A set of button return values for modal dialogs.

typealias ModalSession

Variables of type `NSModalSession` point to information used by the system between `NSApplication`’s beginModalSession(for:) and endModalSession(_:) messages.

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

struct AboutPanelOptionKey

Keys to include in the options dictionary when displaying an About panel.

## See Also

### Managing Windows, Panels, and Menus

App Windows

Show, hide, minimize, arrange, and update your app’s windows.

Menus

Access the app’s main menu items and update the window and services menus.

