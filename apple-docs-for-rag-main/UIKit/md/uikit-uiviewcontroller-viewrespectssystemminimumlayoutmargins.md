

- UIKit
- UIViewController
-  viewRespectsSystemMinimumLayoutMargins 

Instance Property

# viewRespectsSystemMinimumLayoutMargins

A Boolean value indicating whether the view controller’s view uses the system-defined minimum layout margins.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
var viewRespectsSystemMinimumLayoutMargins: Bool { get set }
```

## Mentioned in 

Positioning content within layout margins

## Discussion

When the value of this property is true, the root view’s layout margins are guaranteed to be no smaller than the values in the systemMinimumLayoutMargins property. The default value of this property is true.

Changing this property to false causes the view to obtain its margins solely from its directionalLayoutMargins property. Setting the margins in that property to `0` allows you to eliminate the view’s margins altogether.

## See Also

### Managing the view’s margins

Positioning content within layout margins

Position views so that they aren’t crowded by other content.

var systemMinimumLayoutMargins: NSDirectionalEdgeInsets

The minimum layout margins for the view controller’s root view.

func viewLayoutMarginsDidChange()

Called to notify the view controller that the layout margins of its root view changed.

