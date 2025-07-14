

- UIKit
- UIPopoverPresentationController
-  passthroughViews 

Instance Property

# passthroughViews

An array of views that the user can interact with while the popover is visible.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var passthroughViews: [UIView]? { get set }
```

## Discussion

When a popover is active, interactions with other views are normally disabled until the popover is dismissed. Assigning an array of UIView objects to this property causes UIKit to continue dispatching touch event to the views you specified.

## See Also

### Configuring the popover appearance

var popoverLayoutMargins: UIEdgeInsets

The margins that define the portion of the screen in which it is permissible to display the popover.

var backgroundColor: UIColor?

The color of the popover’s backdrop view.

var popoverBackgroundViewClass: (any UIPopoverBackgroundViewMethods.Type)?

The class to use for displaying the popover background content.

var canOverlapSourceViewRect: Bool

A Boolean value indicating whether the popover can overlap its view rectangle.

