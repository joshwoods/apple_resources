

- AppKit
- NSView
-  getRectsExposedDuringLiveResize(\_:count:) 

Instance Method

# getRectsExposedDuringLiveResize(\_:count:)

Returns a list of rectangles indicating the newly exposed areas of the view.

macOS

``` source
@MainActor
func getRectsExposedDuringLiveResize(
    _ exposedRects: UnsafeMutablePointer,
    count: UnsafeMutablePointer
)
```

## Parameters 

`exposedRects`  

On return, contains the list of rectangles. The returned rectangles are in the coordinate space of the view.

`count`  

Contains the number of rectangles in `exposedRects`; this value may be 0 and is guaranteed to be no more than 4.

## Discussion

If your view does not support content preservation during live resizing, the entire area of your view is returned in the `exposedRects` parameter. To support content preservation, override the preservesContentDuringLiveResize property in your view and have your implementation return true.

Note

The window containing your view must also support content preservation. To enable support for this feature in your window, use the preservesContentDuringLiveResize method of `NSWindow`.

If the view decreased in both height and width, the list of returned rectangles will be empty. If the view increased in both height and width and its upper-left corner stayed anchored in the same position, the list of returned rectangles will contain a vertical and horizontal component indicating the exposed area.

## See Also

### Managing Live Resize

var inLiveResize: Bool

A Boolean value indicating whether the view is being rendered as part of a live resizing operation.

var preservesContentDuringLiveResize: Bool

A Boolean value indicating whether the view optimizes live-resize operations by preserving content that has not moved.

var rectPreservedDuringLiveResize: NSRect

The rectangle identifying the portion of your view that did not change during a live resize operation.

func viewWillStartLiveResize()

Informs the view of the start of a live resize—the user has started resizing the view.

func viewDidEndLiveResize()

Informs the view of the end of a live resize—the user has finished resizing the view.

