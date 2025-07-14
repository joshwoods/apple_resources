

- AppKit
- NSWindow
-  isVisible 

Instance Property

# isVisible

A Boolean value that indicates whether the window is visible onscreen (even when it’s obscured by other windows).

macOS

``` source
@MainActor
var isVisible: Bool { get }
```

## Discussion

The value of this property is true when the window is onscreen (even if it’s obscured by other windows); otherwise, false.

## See Also

### Related Documentation

var visibleRect: NSRect

The portion of the view that isn’t clipped by its superviews.

### Managing Window Visibility and Occlusion State

var occlusionState: NSWindow.OcclusionState

The occlusion state of the window.

