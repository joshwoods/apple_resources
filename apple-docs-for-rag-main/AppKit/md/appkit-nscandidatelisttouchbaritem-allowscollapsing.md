

- AppKit
- NSCandidateListTouchBarItem
-  allowsCollapsing 

Instance Property

# allowsCollapsing

A Boolean value that specifies whether the item can be collapsed.

macOS 10.12.2+

``` source
@MainActor
var allowsCollapsing: Bool { get set }
```

## Discussion

When true, the candidate list item can be collapsed, false otherwise.

The default value is true.

## See Also

### Handling collapsible behavior

var isCollapsed: Bool

A Boolean value that controls the visibility of the candidate list.

