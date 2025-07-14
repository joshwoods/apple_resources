

- UIKit
- UIPopoverPresentationController
-  canOverlapSourceViewRect 

Instance Property

# canOverlapSourceViewRect

A Boolean value indicating whether the popover can overlap its view rectangle.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var canOverlapSourceViewRect: Bool { get set }
```

## Discussion

Setting this property to true allows the popover to overlap the rectangle in the sourceRect property when space is constrained. The default value of this property is false, which prevents the popover from overlapping the source rectangle.

## See Also

### Configuring the popover appearance

var popoverLayoutMargins: UIEdgeInsets

The margins that define the portion of the screen in which it is permissible to display the popover.

var backgroundColor: UIColor?

The color of the popover’s backdrop view.

var passthroughViews: [UIView]?

An array of views that the user can interact with while the popover is visible.

var popoverBackgroundViewClass: (any UIPopoverBackgroundViewMethods.Type)?

The class to use for displaying the popover background content.

