

- UIKit
- UIPopoverPresentationController
-  sourceRect 

Instance Property

# sourceRect

The area in the source view in which you anchor the popover.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var sourceRect: CGRect { get set }
```

## Discussion

Use this property to define the rectangle that the popover’s arrow points to. The rectangle must be in the coordinate space of sourceView.

In iOS 13.2 and later, the default value is CGRectNull, which instructs the system to use the current frame of sourceView. The controller observes changes to this frame and updates the popover accordingly.

In iOS 13.1 and earlier, the default value is zero (Swift) or CGRectZero (Objective-C); using CGRectNull results in undefined behavior.

UIPopoverPresentationController ignores this property if you set the barButtonItem property.

## See Also

### Specifying the popover’s anchor point

var sourceItem: (any UIPopoverPresentationControllerSourceItem)?

The item on which to anchor the popover.

protocol UIPopoverPresentationControllerSourceItem

A type that can be an anchor for a popover presentation controller.

var sourceView: UIView?

The view containing the anchor rectangle for the popover.

var barButtonItem: UIBarButtonItem?

The bar button item on which to anchor the popover.

Deprecated

