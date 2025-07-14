

- AppKit
- NSSplitView
-  isSubviewCollapsed(\_:) 

Instance Method

# isSubviewCollapsed(\_:)

Returns whether the specified view is in a collapsed state.

macOS

``` source
@MainActor
func isSubviewCollapsed(_ subview: NSView) -> Bool
```

## Parameters 

`subview`  

The subview in the split view.

## Return Value

true if `subview` is in a collapsed state; otherwise, false.

## See Also

### Managing Subviews

func adjustSubviews()

Adjusts the sizes of the split view’s subviews so they (plus the dividers) fill the split view.

func holdingPriorityForSubview(at: Int) -> NSLayoutConstraint.Priority

Returns the priority of the subview’s width or height when resizing.

func setHoldingPriority(NSLayoutConstraint.Priority, forSubviewAt: Int)

Sets the priority for split view subviews to maintain their width or height.

