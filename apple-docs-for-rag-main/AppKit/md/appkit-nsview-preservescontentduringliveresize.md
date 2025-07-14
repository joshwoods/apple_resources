

- AppKit
- NSView
-  preservesContentDuringLiveResize 

Instance Property

# preservesContentDuringLiveResize

A Boolean value indicating whether the view optimizes live-resize operations by preserving content that has not moved.

macOS

``` source
@MainActor
var preservesContentDuringLiveResize: Bool { get }
```

## Discussion

The default value of this property is false. If your view supports content preservation, override this property and return true. Content preservation lets your view decide what to redraw during a live resize operation. If your view supports this feature, you should also provide a custom implementation of the setFrameSize(_:) method that invalidates the portions of your view that actually need to be redrawn.

For information on how to implement this feature in your views, see Cocoa Performance Guidelines.

## See Also

### Related Documentation

func setFrameSize(NSSize)

Sets the size of the view’s frame rectangle to the specified dimensions, resizing it within its superview without affecting its coordinate system.

### Managing Live Resize

var inLiveResize: Bool

A Boolean value indicating whether the view is being rendered as part of a live resizing operation.

func getRectsExposedDuringLiveResize(UnsafeMutablePointer&lt;NSRect>, count: UnsafeMutablePointer&lt;Int>)

Returns a list of rectangles indicating the newly exposed areas of the view.

var rectPreservedDuringLiveResize: NSRect

The rectangle identifying the portion of your view that did not change during a live resize operation.

func viewWillStartLiveResize()

Informs the view of the start of a live resize—the user has started resizing the view.

func viewDidEndLiveResize()

Informs the view of the end of a live resize—the user has finished resizing the view.

