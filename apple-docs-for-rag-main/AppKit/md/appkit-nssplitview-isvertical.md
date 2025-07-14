

- AppKit
- NSSplitView
-  isVertical 

Instance Property

# isVertical

A Boolean value that determines the geometric orientation of the split view’s dividers.

macOS

``` source
@MainActor
var isVertical: Bool { get set }
```

## Discussion

The default value of this property is false, which indicates horizontal dividers and views that stack one above the other (top-to-bottom) in the containing split view controller’s view.

To specify vertical dividers and a horizontal (side-by-side) arrangement of views within a split view controller, implement this property to return true.

