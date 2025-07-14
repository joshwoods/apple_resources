

- AppKit
- NSSplitView
-  setHoldingPriority(\_:forSubviewAt:) 

Instance Method

# setHoldingPriority(\_:forSubviewAt:)

Sets the priority for split view subviews to maintain their width or height.

macOS 10.8+

``` source
@MainActor
func setHoldingPriority(
    _ priority: NSLayoutConstraint.Priority,
    forSubviewAt subviewIndex: Int
)
```

## Parameters 

`priority`  

The priority.

`subviewIndex`  

The index of the subview

## Discussion

Calling this method sets the priority that split view subviews use to maintain their width (for a vertical split view) or height (for a horizontal split view). During a split view resize, subviews with higher priorities maintain their sizes before subviews with lower priorities. The subview with the lowest priority is the first to gain additional thickness if the split view grows or shrinks.

The default priority is defaultLow. Use priorities less than dragThatCannotResizeWindow.

## See Also

### Managing Subviews

func adjustSubviews()

Adjusts the sizes of the split view’s subviews so they (plus the dividers) fill the split view.

func isSubviewCollapsed(NSView) -> Bool

Returns whether the specified view is in a collapsed state.

func holdingPriorityForSubview(at: Int) -> NSLayoutConstraint.Priority

Returns the priority of the subview’s width or height when resizing.

