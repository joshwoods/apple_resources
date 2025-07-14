

- AppKit
- NSWindow
-  useOptimizedDrawing(\_:) Deprecated

Instance Method

# useOptimizedDrawing(\_:)

Specifies whether the window is to optimize focusing and drawing when displaying its views.

macOS 10.0–10.10Deprecated

``` source
@MainActor
func useOptimizedDrawing(_ flag: Bool)
```

Deprecated

This method does not do anything and should not be called.

## Parameters 

`flag`  

If true, the window will optimize focusing and drawing for its views; if false, it will not, in which case, the window does not preserve the Z-ordering of overlapping views when an object explicitly sends lockFocus() to a view and draws directly to it, instead of using the AppKit standard display mechanism.

## Discussion

The optimizations may prevent sibling subviews from being displayed in the correct order—which matters only if the subviews overlap. You should always set `flag` to true when there are no overlapping subviews within the window. The default is false.

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

convenience init?(windowRef: UnsafeMutableRawPointer)

Returns a Cocoa window created from a Carbon window.

Deprecated

