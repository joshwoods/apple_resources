

- AppKit
- NSWindow
-  occlusionState 

Instance Property

# occlusionState

The occlusion state of the window.

macOS 10.9+

``` source
@MainActor
var occlusionState: NSWindow.OcclusionState { get }
```

## Discussion

When the value of this property is visible, at least part of the window is visible; otherwise, the window is fully occluded.

## See Also

### Managing Window Visibility and Occlusion State

var isVisible: Bool

A Boolean value that indicates whether the window is visible onscreen (even when it’s obscured by other windows).

