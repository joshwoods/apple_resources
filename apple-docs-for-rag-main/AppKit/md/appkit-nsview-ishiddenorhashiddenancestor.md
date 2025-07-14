

- AppKit
- NSView
-  isHiddenOrHasHiddenAncestor 

Instance Property

# isHiddenOrHasHiddenAncestor

A Boolean value indicating whether the view is hidden from sight because it, or one of its ancestors, is marked as hidden.

macOS

``` source
@MainActor
var isHiddenOrHasHiddenAncestor: Bool { get }
```

## Discussion

The value of this property is true if the value of the isHidden property is true for the current view or any of its ancestors in the view hierarchy. This property does not account for other reasons why a view might be considered hidden, such as being positioned outside its superview’s bounds, not having a window, or residing in a window that is offscreen or overlapped by another window.

## See Also

### Showing and Hiding the View

var isHidden: Bool

A Boolean value indicating whether the view is hidden.

func viewDidHide()

Invoked when the view is hidden, either directly, or in response to an ancestor being hidden.

func viewDidUnhide()

Invoked when the view is unhidden, either directly, or in response to an ancestor being unhidden

