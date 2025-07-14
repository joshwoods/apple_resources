

- UIKit
- UIPopoverPresentationController
-  backgroundColor 

Instance Property

# backgroundColor

The color of the popover’s backdrop view.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+

``` source
@NSCopying @MainActor
var backgroundColor: UIColor? { get set }
```

## Discussion

Use this property to customize the background color of your popover. Changing the value of this property while the popover is visible triggers an animated change to the new color. The default value of this property is `nil`, which corresponds to the default background color.

## See Also

### Configuring the popover appearance

var popoverLayoutMargins: UIEdgeInsets

The margins that define the portion of the screen in which it is permissible to display the popover.

var passthroughViews: [UIView]?

An array of views that the user can interact with while the popover is visible.

var popoverBackgroundViewClass: (any UIPopoverBackgroundViewMethods.Type)?

The class to use for displaying the popover background content.

var canOverlapSourceViewRect: Bool

A Boolean value indicating whether the popover can overlap its view rectangle.

