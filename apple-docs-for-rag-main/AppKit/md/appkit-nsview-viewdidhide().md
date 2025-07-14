

- AppKit
- NSView
-  viewDidHide() 

Instance Method

# viewDidHide()

Invoked when the view is hidden, either directly, or in response to an ancestor being hidden.

macOS 10.5+

``` source
@MainActor
func viewDidHide()
```

## Discussion

The view receives this message when its isHiddenOrHasHiddenAncestor property changes from false to true. This happens when the view or an ancestor is marked as hidden, or when the view or an ancestor is inserted into a new view hierarchy.

## See Also

### Showing and Hiding the View

var isHidden: Bool

A Boolean value indicating whether the view is hidden.

var isHiddenOrHasHiddenAncestor: Bool

A Boolean value indicating whether the view is hidden from sight because it, or one of its ancestors, is marked as hidden.

func viewDidUnhide()

Invoked when the view is unhidden, either directly, or in response to an ancestor being unhidden

