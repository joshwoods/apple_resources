

- AppKit
-  NSWindowDelegate 

Protocol

# NSWindowDelegate

A set of optional methods that a window’s delegate can implement to respond to events, such as window resizing, moving, exposing, and minimizing.

macOS

``` source
protocol NSWindowDelegate : NSObjectProtocol
```

## Topics

### Managing Sheets

func window(NSWindow, willPositionSheet: NSWindow, using: NSRect) -> NSRect

Tells the delegate that the window is about to show a sheet at the specified location, giving it the opportunity to return a custom location for the attachment of the sheet to the window.

func windowWillBeginSheet(Notification)

Notifies the delegate that the window is about to open a sheet.

func windowDidEndSheet(Notification)

Tells the delegate that the window has closed a sheet.

### Sizing Windows

func windowWillResize(NSWindow, to: NSSize) -> NSSize

Tells the delegate that the window is being resized (whether by the user or through one of the `setFrame...` methods other than setFrame(_:display:)).

func windowDidResize(Notification)

Tells the delegate that the window has been resized.

func windowWillStartLiveResize(Notification)

Tells the delegate that the window is about to be live resized.

func windowDidEndLiveResize(Notification)

Tells the delegate that a live resize operation on the window has ended.

### Minimizing Windows

func windowWillMiniaturize(Notification)

Tells the delegate that the window is about to be minimized.

func windowDidMiniaturize(Notification)

Tells the delegate that the window has been minimized.

func windowDidDeminiaturize(Notification)

Tells the delegate that the window has been deminimized.

### Zooming Window

func windowWillUseStandardFrame(NSWindow, defaultFrame: NSRect) -> NSRect

Called by `NSWindow`’s zoom(_:) method while determining the frame a window may be zoomed to.

func windowShouldZoom(NSWindow, toFrame: NSRect) -> Bool

Asks the delegate whether the specified window should zoom to the specified frame.

### Managing Full-Screen Presentation

func window(NSWindow, willUseFullScreenContentSize: NSSize) -> NSSize

Called to allow the delegate to modify the full-screen content size.

func window(NSWindow, willUseFullScreenPresentationOptions: NSApplication.PresentationOptions) -> NSApplication.PresentationOptions

Returns the presentation options the window uses when transitioning to full-screen mode.

func windowWillEnterFullScreen(Notification)

The window is about to enter full-screen mode.

func windowDidEnterFullScreen(Notification)

The window has entered full-screen mode.

func windowWillExitFullScreen(Notification)

The window is about to exit full-screen mode.

func windowDidExitFullScreen(Notification)

The window has left full-screen mode.

### Custom Full-Screen Presentation Animations

func customWindowsToEnterFullScreen(for: NSWindow) -> [NSWindow]?

Called when the window is about to enter full-screen mode.

func customWindowsToEnterFullScreen(for: NSWindow, on: NSScreen) -> [NSWindow]?

Called when the window is about to enter full-screen mode.

func window(NSWindow, startCustomAnimationToEnterFullScreenWithDuration: TimeInterval)

This method is called to start the window animation into full-screen mode, including transitioning to a new space.

func window(NSWindow, startCustomAnimationToEnterFullScreenOn: NSScreen, withDuration: TimeInterval)

This method is called to start the window animation into full-screen mode, including transitioning to a new space.

func windowDidFailToEnterFullScreen(NSWindow)

Called if the window failed to enter full-screen mode.

func customWindowsToExitFullScreen(for: NSWindow) -> [NSWindow]?

Called when the window is about to exit full-screen mode.

func window(NSWindow, startCustomAnimationToExitFullScreenWithDuration: TimeInterval)

This method is called to start the window animation out of full-screen mode, including transitioning back to the desktop space.

func windowDidFailToExitFullScreen(NSWindow)

Called if the window failed to exit full-screen mode.

### Moving Windows

func windowWillMove(Notification)

Tells the delegate that the window is about to move.

func windowDidMove(Notification)

Tells the delegate that the window has moved.

func windowDidChangeScreen(Notification)

Tells the delegate that the window has changed screens.

func windowDidChangeScreenProfile(Notification)

Tells the delegate that the window has changed screen display profiles.

func windowDidChangeBackingProperties(Notification)

Tells the delegate that the window backing properties changed.

### Closing Windows

func windowShouldClose(NSWindow) -> Bool

Tells the delegate that the user has attempted to close a window or the window has received a performClose(_:) message.

func windowWillClose(Notification)

Tells the delegate that the window is about to close.

### Managing Key Status

func windowDidBecomeKey(Notification)

Tells the delegate that the window has become the key window.

func windowDidResignKey(Notification)

Tells the delegate that the window has resigned key window status.

### Managing Main Status

func windowDidBecomeMain(Notification)

Tells the delegate that the window has become main.

func windowDidResignMain(Notification)

Tells the delegate that the window has resigned main window status.

### Managing Field Editors

func windowWillReturnFieldEditor(NSWindow, to: Any?) -> Any?

Tells the delegate that the field editor for a text-displaying object has been requested.

### Updating Windows

func windowDidUpdate(Notification)

Tells the delegate that the window received an update() message.

### Exposing Windows

func windowDidExpose(Notification)

Tells the delegate that the window has been exposed.

### Managing Occlusion State

func windowDidChangeOcclusionState(Notification)

Tells the delegate that the window changed its occlusion state.

### Dragging Windows

func window(NSWindow, shouldDragDocumentWith: NSEvent, from: NSPoint, with: NSPasteboard) -> Bool

Asks the delegate whether a user can drag the document icon from the window’s title bar.

### Getting the Undo Manager

func windowWillReturnUndoManager(NSWindow) -> UndoManager?

Tells the delegate that the window’s undo manager has been requested. Returns the appropriate undo manager for the window.

### Managing Titles

func window(NSWindow, shouldPopUpDocumentPathMenu: NSMenu) -> Bool

Asks the delegate whether the window displays the title pop-up menu in response to a Command-click or Control-click on its title.

### Managing Restorable State

func window(NSWindow, willEncodeRestorableState: NSCoder)

Tells the delegate the window is about to add its restorable state to a given archiver.

func window(NSWindow, didDecodeRestorableState: NSCoder)

Tells the delegate the window is has extracted its restorable state from a given archiver.

### Managing Presentation in Version Browsers

func window(NSWindow, willResizeForVersionBrowserWithMaxPreferredSize: NSSize, maxAllowedSize: NSSize) -> NSSize

Tells the delegate the window will resize for presentation during version browsing.

func windowWillEnterVersionBrowser(Notification)

Tells the delegate the window is about to enter version browsing.

func windowDidEnterVersionBrowser(Notification)

Tells the delegate that the window has entered version browsing.

func windowWillExitVersionBrowser(Notification)

Tells the delegate that the window is about to leave version browsing.

func windowDidExitVersionBrowser(Notification)

Tells the delegate that the window has left version browsing.

### Instance Methods

func previewRepresentableActivityItems(for: NSWindow) -> [any NSPreviewRepresentableActivityItem]?

func windowForSharingRequest(from: NSWindow) -> NSWindow?

Method called to get the window to share once sharing is confirmed, after a request is initiated by requestSharingOfWindowUsingPreview:title:completionHandler:. Implement this on the delegate of the requesting window

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Windows

class NSWindow

A window that an app displays on the screen.

class NSPanel

A special kind of window that typically performs a function that is auxiliary to the main window.

class NSWindowTab

A tab associated with a window that is part of a tabbing group.

class NSWindowTabGroup

A group of windows that display together as a single tabbed window.

