

- AppKit
- NSCandidateListTouchBarItem
-  isCollapsed 

Instance Property

# isCollapsed

A Boolean value that controls the visibility of the candidate list.

macOS 10.12.2+

``` source
@MainActor
var isCollapsed: Bool { get set }
```

## Discussion

When true, the candidate list is collapsed and not visible to the user.

The default value is true.

## See Also

### Handling collapsible behavior

var allowsCollapsing: Bool

A Boolean value that specifies whether the item can be collapsed.

