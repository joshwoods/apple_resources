

- AppKit
- NSWindow
-  init(windowRef:) Deprecated

Initializer

# init(windowRef:)

Returns a Cocoa window created from a Carbon window.

macOS 10.0–15.0Deprecated

``` source
@MainActor
convenience init?(windowRef: UnsafeMutableRawPointer)
```

Deprecated

This method should not be used.

## Parameters 

`windowRef`  

The Carbon `WindowRef` object to use to create the Cocoa window.

## Return Value

A Cocoa window created from `windowRef`.

## Discussion

For more information on Carbon-Cocoa integration, see Using a Carbon User Interface in a Cocoa Application in Carbon-Cocoa Integration Guide.

### Special Considerations

For historical reasons, contrary to normal memory management policy `initWithWindowRef:` does *not* retain `windowRef`. It is therefore recommended that you make sure you retain `windowRef` before calling this method. If `windowRef` is still valid when the Cocoa window is deallocated, the Cocoa window will release it.

## See Also

### Related Documentation

class NSWindow

A window that an app displays on the screen.

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

