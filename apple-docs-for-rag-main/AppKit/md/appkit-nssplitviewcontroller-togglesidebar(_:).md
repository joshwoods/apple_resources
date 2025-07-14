

- AppKit
- NSSplitViewController
-  toggleSidebar(\_:) 

Instance Method

# toggleSidebar(\_:)

Collapses or expands the first sidebar in the split view controller using an animation.

macOS 10.11+

``` source
@IBAction @MainActor
func toggleSidebar(_ sender: Any?)
```

## Discussion

If the split view controller doesn’t contain a sidebar, calling this method does nothing.

## See Also

### Managing Sidebars

var minimumThicknessForInlineSidebars: CGFloat

The minimum thickness for a sidebar before it automatically collapses.

class let automaticDimension: CGFloat

The default value to apply to a dimension.

