

- UIKit
- UIViewController
-  systemMinimumLayoutMargins 

Instance Property

# systemMinimumLayoutMargins

The minimum layout margins for the view controller’s root view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
var systemMinimumLayoutMargins: NSDirectionalEdgeInsets { get }
```

## Mentioned in 

Positioning content within layout margins

## Discussion

This property contains the minimum layout margins expected by the system for the view controller’s root view. Do not override this property. To stop considering the system’s minimum layout margins for the root view, set the viewRespectsSystemMinimumLayoutMargins property to false. This property does not affect the margins associated with subviews of the root view.

If you assign a custom value to the directionalLayoutMargins property of the view controller’s root view, the root view’s actual margins are set to either your custom values or the minimum values defined by this property, whichever values are greater. For example, if the value for one system minimum margin is `20` points and you specify a value of `10` for the same margin on the view, the view uses the value `20` for the margin.

## See Also

### Managing the view’s margins

Positioning content within layout margins

Position views so that they aren’t crowded by other content.

var viewRespectsSystemMinimumLayoutMargins: Bool

A Boolean value indicating whether the view controller’s view uses the system-defined minimum layout margins.

func viewLayoutMarginsDidChange()

Called to notify the view controller that the layout margins of its root view changed.

