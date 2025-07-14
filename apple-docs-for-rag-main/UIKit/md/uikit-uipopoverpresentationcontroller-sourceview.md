

- UIKit
- UIPopoverPresentationController
-  sourceView 

Instance Property

# sourceView

The view containing the anchor rectangle for the popover.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var sourceView: UIView? { get set }
```

## Discussion

Use this property in conjunction with the sourceRect property to specify the anchor location for the popover. Alternatively, you may specify the anchor location for the popover using the barButtonItem property.

## See Also

### Specifying the popover’s anchor point

var sourceItem: (any UIPopoverPresentationControllerSourceItem)?

The item on which to anchor the popover.

protocol UIPopoverPresentationControllerSourceItem

A type that can be an anchor for a popover presentation controller.

var sourceRect: CGRect

The area in the source view in which you anchor the popover.

var barButtonItem: UIBarButtonItem?

The bar button item on which to anchor the popover.

Deprecated

