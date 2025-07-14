

- UIKit
- UIPopoverPresentationController
-  sourceItem 

Instance Property

# sourceItem

The item on which to anchor the popover.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
var sourceItem: (any UIPopoverPresentationControllerSourceItem)? { get set }
```

## Discussion

Assign a value to this property to anchor the popover to the specified UIBarButtonItem or NSToolbarItem. When presented, the popover’s arrow points to the specified item. Alternatively, you may specify the anchor location for the popover using the sourceView and sourceRect properties.

The default value of this property is `nil`.

## See Also

### Specifying the popover’s anchor point

protocol UIPopoverPresentationControllerSourceItem

A type that can be an anchor for a popover presentation controller.

var sourceView: UIView?

The view containing the anchor rectangle for the popover.

var sourceRect: CGRect

The area in the source view in which you anchor the popover.

var barButtonItem: UIBarButtonItem?

The bar button item on which to anchor the popover.

Deprecated

