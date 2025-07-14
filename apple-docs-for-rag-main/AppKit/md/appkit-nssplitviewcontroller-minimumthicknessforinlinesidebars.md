

- AppKit
- NSSplitViewController
-  minimumThicknessForInlineSidebars 

Instance Property

# minimumThicknessForInlineSidebars

The minimum thickness for a sidebar before it automatically collapses.

macOS 10.11+

``` source
@MainActor
var minimumThicknessForInlineSidebars: CGFloat { get set }
```

## Discussion

This value describes the minimum thickness in the primary axis of a split view—width if the split view’s isVertical value is true, height if it’s false. This value is the minimum thickness that sidebars can shrink to before they automatically collapse. When sidebars autocollapse in full-screen mode, they overlay the other split view items.

Autocollapsed sidebars automatically expand if their thickness increases to or above this minimum thickness threshold.

The default value of this property is automaticDimension, which determines the minimum thickness for sidebars using the effective minimum size of the split view item views from the layout constraints in the window. If the system can’t apply the constraints that establish the minimum size for all noncollapsed split panes, all sidebars automatically collapse. In full-screen mode, if a sidebar attempts to expand in this state, it overlays instead.

## See Also

### Managing Sidebars

func toggleSidebar(Any?)

Collapses or expands the first sidebar in the split view controller using an animation.

class let automaticDimension: CGFloat

The default value to apply to a dimension.

