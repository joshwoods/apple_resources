

- AppKit
- NSWindow
-  cacheImage(in:) Deprecated

Instance Method

# cacheImage(in:)

Stores the window’s raster image from a given rectangle expressed in the window’s base coordinate system.

macOS 10.0–10.13Deprecated

``` source
@MainActor
func cacheImage(in rect: NSRect)
```

Deprecated

This method shouldn’t be used as it doesn’t work in all drawing situations; instead, a subview should be used that implements the desired drawing behavior

## Parameters 

`rect`  

The rectangle representing the image to cache.

## Discussion

This method allows the window to perform temporary drawing, such as a band around the selection as the user drags the mouse, and to quickly restore the previous image by invoking restoreCachedImage() and flushIfNeeded(). The next time the window displays, it discards its cached image rectangles. You can also explicitly use discardCachedImage() to free the memory occupied by cached image rectangles. `rect` is made integral before caching the image to avoid antialiasing artifacts.

Only the last cached rectangle is remembered and can be restored.

## See Also

### Related Documentation

func display()

Passes a display message down the window’s view hierarchy, thus redrawing all views within the window.

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

