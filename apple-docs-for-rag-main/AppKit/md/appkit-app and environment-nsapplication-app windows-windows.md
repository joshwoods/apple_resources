

- AppKit
- App and Environment
- NSApplication
-  App Windows 

API Collection

# App Windows

Show, hide, minimize, arrange, and update your app’s windows.

## Topics

### Managing App Windows

var keyWindow: NSWindow?

The window that currently receives keyboard events.

var mainWindow: NSWindow?

The app’s main window.

func window(withWindowNumber: Int) -> NSWindow?

Returns the window corresponding to the specified window number.

var windows: [NSWindow]

An array of the app’s window objects.

func makeWindowsPerform(Selector, inOrder: Bool) -> NSWindow?

Sends the specified message to each of the app’s window objects until one returns a non-`nil` value.

Deprecated

func enumerateWindows(options: NSApplication.WindowListOptions, using: (NSWindow, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes a block for each of the app’s windows.

struct WindowListOptions

This constant indicates a window ordering.

### Minimizing Windows

func miniaturizeAll(Any?)

Miniaturizes all the receiver’s windows.

### Hiding Windows

var isHidden: Bool

A Boolean value indicating whether the app is hidden.

func hide(Any?)

Hides all the receiver’s windows, and the next app in line is activated.

func unhide(Any?)

Restores hidden windows to the screen and makes the receiver active.

func unhideWithoutActivation()

Restores hidden windows without activating their owner (the receiver).

### Updating Windows

func updateWindows()

Sends an update() message to each onscreen window.

func setWindowsNeedUpdate(Bool)

Sets whether the receiver’s windows need updating when the receiver has finished processing the current event.

### Managing Window Layers

func preventWindowOrdering()

Suppresses the usual window ordering in handling the most recent mouse-down event.

func arrangeInFront(Any?)

Arranges windows listed in the Window menu in front of all other windows.

### Drawing Windows

var context: NSGraphicsContext?

The graphics context associated with the app.

Deprecated

### Getting the Occlusion State

var occlusionState: NSApplication.OcclusionState

The occlusion state of the app.

struct OcclusionState

This constant indicates whether at least part of any window owned by this app is visible.

### Restoring App Windows at Launch

var isProtectedDataAvailable: Bool

func extendStateRestoration()

Allows an app to extend its state restoration period.

func completeStateRestoration()

Completes the extended state restoration.

func restoreWindow(withIdentifier: NSUserInterfaceItemIdentifier, state: NSCoder, completionHandler: (NSWindow?, (any Error)?) -> Void) -> Bool

Invoked to request that a window be restored.

### Managing Run Loops

class var displayWindowRunLoopOrdering: Int

The priority at which windows are displayed.

class var resetCursorRectsRunLoopOrdering: Int

The priority at which cursor rects are reset.

NSUpdateWindowsRunLoopOrdering

This constant is used by the `NSRunLoop` method perform(_:target:argument:order:modes:).

## See Also

### Managing Windows, Panels, and Menus

Modal Windows and Panels

Display a modal window or show one of the standard app panels, such as the app’s About panel.

Menus

Access the app’s main menu items and update the window and services menus.

