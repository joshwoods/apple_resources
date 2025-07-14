

- UIKit
- UIViewController
-  viewLayoutMarginsDidChange() 

Instance Method

# viewLayoutMarginsDidChange()

Called to notify the view controller that the layout margins of its root view changed.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
func viewLayoutMarginsDidChange()
```

## Mentioned in 

Displaying and managing views with a view controller

## Discussion

Use this method to update the position of content based on the new margin values.

## See Also

### Managing the view’s margins

Positioning content within layout margins

Position views so that they aren’t crowded by other content.

var viewRespectsSystemMinimumLayoutMargins: Bool

A Boolean value indicating whether the view controller’s view uses the system-defined minimum layout margins.

var systemMinimumLayoutMargins: NSDirectionalEdgeInsets

The minimum layout margins for the view controller’s root view.

