

- UIKit
- UIPopoverPresentationController
-  popoverBackgroundViewClass 

Instance Property

# popoverBackgroundViewClass

The class to use for displaying the popover background content.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var popoverBackgroundViewClass: (any UIPopoverBackgroundViewMethods.Type)? { get set }
```

## Discussion

The default value of this property is `nil`, which causes the presentation controller to use the default popover appearance. Setting this property to a value other than `nil` causes the presentation controller to use the specified class to draw the popover’s background content. The class you specify must be a subclass of UIPopoverBackgroundView.

## See Also

### Configuring the popover appearance

var popoverLayoutMargins: UIEdgeInsets

The margins that define the portion of the screen in which it is permissible to display the popover.

var backgroundColor: UIColor?

The color of the popover’s backdrop view.

var passthroughViews: [UIView]?

An array of views that the user can interact with while the popover is visible.

var canOverlapSourceViewRect: Bool

A Boolean value indicating whether the popover can overlap its view rectangle.

