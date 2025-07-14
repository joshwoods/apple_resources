

- AppKit
- NSView
-  viewDidUnhide() 

Instance Method

# viewDidUnhide()

Invoked when the view is unhidden, either directly, or in response to an ancestor being unhidden

macOS 10.5+

``` source
@MainActor
func viewDidUnhide()
```

## Discussion

The view receives this message when its `isHiddenOrHasHiddenAncestor` state goes from true to false.  This can happen when the view or an ancestor is marked as not hidden, or when the view or an ancestor is removed from its containing view hierarchy.

## See Also

### Showing and Hiding the View

var isHidden: Bool

A Boolean value indicating whether the view is hidden.

var isHiddenOrHasHiddenAncestor: Bool

A Boolean value indicating whether the view is hidden from sight because it, or one of its ancestors, is marked as hidden.

func viewDidHide()

Invoked when the view is hidden, either directly, or in response to an ancestor being hidden.

