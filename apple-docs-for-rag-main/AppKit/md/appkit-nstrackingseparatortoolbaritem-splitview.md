

- AppKit
- NSTrackingSeparatorToolbarItem
-  splitView 

Instance Property

# splitView

The vertical split view to align with the toolbar separator.

macOS 11.0+

``` source
@MainActor
var splitView: NSSplitView { get set }
```

## Discussion

The `splitView` must be in the same window as the toolbar containing the `NSTrackingSeparatorToolbarItem` before showing the toolbar.

## See Also

### configuring a tracking separator

var dividerIndex: Int

The index of the split view divider to align with the tracking separator.

