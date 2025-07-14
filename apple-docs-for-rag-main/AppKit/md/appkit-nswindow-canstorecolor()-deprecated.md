

- AppKit
- NSWindow
-  canStoreColor() Deprecated

Instance Method

# canStoreColor()

Indicates whether the window has a depth limit that allows it to store color values.

macOS 10.0–10.10Deprecated

``` source
@MainActor
func canStoreColor() -> Bool
```

Deprecated

This method does not do anything and should not be called.

## Return Value

true when the window’s depth limit allows it to store color values; otherwise, false.

## See Also

### Related Documentation

func shouldDrawColor() -> Bool

Returns a Boolean value indicating whether the view is being drawn to an environment that supports color.

Deprecated

var depthLimit: NSWindow.Depth

The depth limit of the window.

### Methods

func gState() -> Int

Returns the window’s graphics state object.

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

