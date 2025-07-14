

- UIKit
- UINavigationItem
-  overflowPresentationSource 

Instance Property

# overflowPresentationSource

The item you can use as an anchor to present a custom UI from the overflow menu button.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
var overflowPresentationSource: (any UIPopoverPresentationControllerSourceItem)? { get }
```

## Discussion

If the overflow menu button for the navigation item is visible, this property returns a non-`nil` item that you can use as a presentation source — for example, to present a custom popover that anchors to the overflow menu button. Otherwise, this property returns `nil`.

## See Also

### Working with the overflow menu

var additionalOverflowItems: UIDeferredMenuElement?

Additional items to present in the overflow menu.

