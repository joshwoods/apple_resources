

- AppKit
- NSWindow
-  disableFlushing() Deprecated

Instance Method

# disableFlushing()

Disables the flush() method for the window.

macOS 10.0–10.14Deprecated

``` source
@MainActor
func disableFlushing()
```

Deprecated

Use +\[NSAnimationContext runAnimationGroup:completionHandler:\] to perform atomic updates across runloop invocations.

## Discussion

If the window is buffered, disabling flush() prevents drawing from being automatically flushed by the `NSView` `display...` methods from the window’s backing store to the screen. This method permits several views to be drawn before the results are shown to the user.

Flushing should be disabled only temporarily, while the window’s display is being updated. Each `disableFlushWindow` message must be paired with a subsequent enableFlushing() message. Invocations of these methods can be nested; flushing isn’t reenabled until the last enableFlushing() message is sent.

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

