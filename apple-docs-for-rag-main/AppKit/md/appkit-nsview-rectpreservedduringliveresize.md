

- AppKit
- NSView
-  rectPreservedDuringLiveResize 

Instance Property

# rectPreservedDuringLiveResize

The rectangle identifying the portion of your view that did not change during a live resize operation.

macOS

``` source
@MainActor
var rectPreservedDuringLiveResize: NSRect { get }
```

## Discussion

The rectangle in this property is in the coordinate system of your view and reflects the space your view previously occupied. This rectangle may be smaller or the same size as your view’s current bounds, depending on whether the view grew or shrunk.

If your view does not support content preservation during live resizing, the rectangle will be empty. To support content preservation, override the preservesContentDuringLiveResize property in your view and have your implementation return true.

Note

The window containing your view must also support content preservation. To enable support for this feature in your window, use the preservesContentDuringLiveResize method of `NSWindow`.

## See Also

### Managing Live Resize

var inLiveResize: Bool

A Boolean value indicating whether the view is being rendered as part of a live resizing operation.

var preservesContentDuringLiveResize: Bool

A Boolean value indicating whether the view optimizes live-resize operations by preserving content that has not moved.

func getRectsExposedDuringLiveResize(UnsafeMutablePointer&lt;NSRect>, count: UnsafeMutablePointer&lt;Int>)

Returns a list of rectangles indicating the newly exposed areas of the view.

func viewWillStartLiveResize()

Informs the view of the start of a live resize—the user has started resizing the view.

func viewDidEndLiveResize()

Informs the view of the end of a live resize—the user has finished resizing the view.

