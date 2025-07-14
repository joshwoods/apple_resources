

- AppKit
- NSView
-  viewWillStartLiveResize() 

Instance Method

# viewWillStartLiveResize()

Informs the view of the start of a live resize—the user has started resizing the view.

macOS

``` source
@MainActor
func viewWillStartLiveResize()
```

## Discussion

In the simple case, a view is sent viewWillStartLiveResize() before the first resize operation on the containing window and viewDidEndLiveResize() after the last resize operation. A view that is repeatedly added and removed from a window during live resize will receive only one viewWillStartLiveResize() (on the first time it is added to the window) and one viewDidEndLiveResize() (when the window has completed the live resize operation). This allows a superview such as NSBrowser object to add and remove its `NSMatrix` subviews during live resize without the NSMatrix object receiving multiple calls to these methods.

A view might allocate data structures to cache-drawing information in viewWillStartLiveResize() and should clean up these data structures in viewDidEndLiveResize(). In addition, a view that does optimized drawing during live resize might need to do full drawing after viewDidEndLiveResize(). However, you should not assume that a view has a drawing context in viewDidEndLiveResize() (since it may have been removed from the window during live resize). A view that needs to redraw itself after live resize should set its needsDisplay property to true in viewDidEndLiveResize().

A view subclass should call `super` from these methods.

## See Also

### Managing Live Resize

var inLiveResize: Bool

A Boolean value indicating whether the view is being rendered as part of a live resizing operation.

var preservesContentDuringLiveResize: Bool

A Boolean value indicating whether the view optimizes live-resize operations by preserving content that has not moved.

func getRectsExposedDuringLiveResize(UnsafeMutablePointer&lt;NSRect>, count: UnsafeMutablePointer&lt;Int>)

Returns a list of rectangles indicating the newly exposed areas of the view.

var rectPreservedDuringLiveResize: NSRect

The rectangle identifying the portion of your view that did not change during a live resize operation.

func viewDidEndLiveResize()

Informs the view of the end of a live resize—the user has finished resizing the view.

