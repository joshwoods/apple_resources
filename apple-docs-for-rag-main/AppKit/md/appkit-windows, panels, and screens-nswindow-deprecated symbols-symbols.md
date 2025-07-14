

- AppKit
- Windows, Panels, and Screens
- NSWindow
-  Deprecated Symbols 

API Collection

# Deprecated Symbols

Review unsupported symbols and their replacements.

## Topics

### Methods

func gState() -> Int

Returns the window’s graphics state object.

Deprecated

func canStoreColor() -> Bool

Indicates whether the window has a depth limit that allows it to store color values.

Deprecated

func enableFlushing()

Reenables the flush() method for the window after it was disabled through a previous disableFlushing() message.

Deprecated

func disableFlushing()

Disables the flush() method for the window.

Deprecated

func flush()

Flushes the window’s offscreen buffer to the screen if the window is buffered and flushing is enabled.

Deprecated

func flushIfNeeded()

Flushes the window’s offscreen buffer to the screen if flushing is enabled and if the last flush() message had no effect because flushing was disabled.

Deprecated

class func menuChanged(NSMenu)

This method does nothing; it is here for backward compatibility.

Deprecated

func cacheImage(in: NSRect)

Stores the window’s raster image from a given rectangle expressed in the window’s base coordinate system.

Deprecated

func restoreCachedImage()

Splices the window’s cached image rectangles, if any, back into its raster image (and buffer if it has one), undoing the effect of any drawing performed within those areas since they were established using cacheImage(in:).

Deprecated

func discardCachedImage()

Discards all of the window’s cached image rectangles.

Deprecated

func useOptimizedDrawing(Bool)

Specifies whether the window is to optimize focusing and drawing when displaying its views.

Deprecated

convenience init?(windowRef: UnsafeMutableRawPointer)

Returns a Cocoa window created from a Carbon window.

Deprecated

### Properties

var backingLocation: NSWindow.BackingLocation

The location of the window’s backing store.

Deprecated

var preferredBackingLocation: NSWindow.BackingLocation

A Boolean value that indicates the preferred location for the window’s backing store.

Deprecated

var isOneShot: Bool

A Boolean value that indicates whether the window device the window manages is freed when it’s removed from the screen list.

Deprecated

var drawers: [NSDrawer]?

The collection of drawers associated with the window.

Deprecated

var showsResizeIndicator: Bool

A Boolean value that indicates whether the window’s resize indicator is visible.

Deprecated

var isFlushWindowDisabled: Bool

A Boolean value that indicates whether the window’s flushing ability is disabled.

Deprecated

var isAutodisplay: Bool

A Boolean value that indicates whether the window automatically displays views that need to be displayed.

Deprecated

var graphicsContext: NSGraphicsContext?

The graphics context associated with the window for the current thread.

Deprecated

var windowRef: UnsafeMutableRawPointer

The Carbon window reference associated with the window, creating one if necessary.

Deprecated

### Constants

enum BackingLocation

The following constants and the related data type represent a window’s possible backing locations.

Deprecated

