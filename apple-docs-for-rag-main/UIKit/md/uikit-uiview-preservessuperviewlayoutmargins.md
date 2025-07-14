

- UIKit
- UIView
-  preservesSuperviewLayoutMargins 

Instance Property

# preservesSuperviewLayoutMargins

A Boolean value indicating whether the current view also respects the margins of its superview.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var preservesSuperviewLayoutMargins: Bool { get set }
```

## Mentioned in 

Positioning content within layout margins

## Discussion

When the value of this property is true, the superview’s margins are also considered when laying out content. This margin affects layouts where the distance between the edge of a view and its superview is smaller than the corresponding margin. For example, you might have a content view whose frame precisely matches the bounds of its superview. When any of the superview’s margins is inside the area represented by the content view and its own margins, UIKit adjusts the content view’s layout to respect the superview’s margins. The amount of the adjustment is the smallest amount needed to ensure that content is also inside the superview’s margins.

The default value of this property is false.

## See Also

### Configuring content margins

Positioning content within layout margins

Position views so that they aren’t crowded by other content.

var directionalLayoutMargins: NSDirectionalEdgeInsets

The default spacing to use when laying out content in a view, taking into account the current language direction.

var layoutMargins: UIEdgeInsets

The default spacing to use when laying out content in the view.

func layoutMarginsDidChange()

Notifies the view that the layout margins changed.

