

- AppKit
- NSView
-  inLiveResize 

Instance Property

# inLiveResize

A Boolean value indicating whether the view is being rendered as part of a live resizing operation.

macOS

``` source
@MainActor
var inLiveResize: Bool { get }
```

## Discussion

AppKit sets the value of this property to true when a live resizing operation involving the view is underway. Use this property to determine when to optimize your view’s drawing behavior. Typically, you access this property from your draw(_:) method and use the value to change the fidelity of the content you draw, or to draw your content more efficiently.

## See Also

### Managing Live Resize

var preservesContentDuringLiveResize: Bool

A Boolean value indicating whether the view optimizes live-resize operations by preserving content that has not moved.

func getRectsExposedDuringLiveResize(UnsafeMutablePointer&lt;NSRect>, count: UnsafeMutablePointer&lt;Int>)

Returns a list of rectangles indicating the newly exposed areas of the view.

var rectPreservedDuringLiveResize: NSRect

The rectangle identifying the portion of your view that did not change during a live resize operation.

func viewWillStartLiveResize()

Informs the view of the start of a live resize—the user has started resizing the view.

func viewDidEndLiveResize()

Informs the view of the end of a live resize—the user has finished resizing the view.

