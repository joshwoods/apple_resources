

- AppKit
- NSWindow
-  flush() Deprecated

Instance Method

# flush()

Flushes the window’s offscreen buffer to the screen if the window is buffered and flushing is enabled.

macOS 10.0–10.14Deprecated

``` source
@MainActor
func flush()
```

Deprecated

Allow AppKit's automatic deferred display mechanism to take care of flushing any graphics contexts as needed.

## Discussion

Does nothing for other display devices, such as a printer. This method is automatically invoked by the `NSWindow` display() and displayIfNeeded() methods and the corresponding NSView display() and displayIfNeeded() methods.

## See Also

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

