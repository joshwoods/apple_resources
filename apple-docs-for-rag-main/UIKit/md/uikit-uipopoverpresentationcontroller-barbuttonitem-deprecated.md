

- UIKit
- UIPopoverPresentationController
-  barButtonItem Deprecated

Instance Property

# barButtonItem

The bar button item on which to anchor the popover.

iOS 8.0–18.4DeprecatediPadOS 8.0–18.4DeprecatedMac Catalyst 13.1+visionOS 1.0–2.4Deprecated

``` source
@MainActor
var barButtonItem: UIBarButtonItem? { get set }
```

Deprecated

Use the sourceItem property to anchor the popover to a UIBarButtonItem instead.

## Discussion

Assign a value to this property to anchor the popover to the specified bar button item. When presented, the popover’s arrow points to the specified item. Alternatively, you may specify the anchor location for the popover using the sourceView and sourceRect properties.

Prior to presentation, the presentation controller adds all sibling bar button items of the specified item (but not the item itself) to the popover’s list of passthrough views. UIKit automatically intercepts taps in the specified item and uses them to dismiss the popover. If you want taps in the other bar button items to dismiss the popover, you must add code to the action handlers of those items.

The default value of this property is `nil`.

## See Also

### Specifying the popover’s anchor point

var sourceItem: (any UIPopoverPresentationControllerSourceItem)?

The item on which to anchor the popover.

protocol UIPopoverPresentationControllerSourceItem

A type that can be an anchor for a popover presentation controller.

var sourceView: UIView?

The view containing the anchor rectangle for the popover.

var sourceRect: CGRect

The area in the source view in which you anchor the popover.

