

- UIKit
- UIView
-  layoutMarginsDidChange() 

Instance Method

# layoutMarginsDidChange()

Notifies the view that the layout margins changed.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func layoutMarginsDidChange()
```

## Discussion

The default implementation of this method does nothing. Subclasses can override this method and use it to respond when the value in the view’s layoutMargins property changes. For example, you might override this method if your view subclass handles layout manually or uses the layout margins during drawing. In both cases, you could use this method to initiate a drawing or layout update.

## See Also

### Configuring content margins

Positioning content within layout margins

Position views so that they aren’t crowded by other content.

var directionalLayoutMargins: NSDirectionalEdgeInsets

The default spacing to use when laying out content in a view, taking into account the current language direction.

var layoutMargins: UIEdgeInsets

The default spacing to use when laying out content in the view.

var preservesSuperviewLayoutMargins: Bool

A Boolean value indicating whether the current view also respects the margins of its superview.

