

- UIKit
- UINavigationItem
-  additionalOverflowItems 

Instance Property

# additionalOverflowItems

Additional items to present in the overflow menu.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
var additionalOverflowItems: UIDeferredMenuElement? { get set }
```

## Discussion

When you assign a non-`nil` value to this property, the overflow menu button appears on the trailing edge of the navigation bar. This button appears regardless of whether you provide menu elements in the callback for the UIDeferredMenuElement.

The system presents any menu elements you return in the callback for UIDeferredMenuElement in the overflow menu. The system also populates the overflow menu with any items that can’t fit in the navigation bar due to layout space constraints.

## See Also

### Working with the overflow menu

var overflowPresentationSource: (any UIPopoverPresentationControllerSourceItem)?

The item you can use as an anchor to present a custom UI from the overflow menu button.

