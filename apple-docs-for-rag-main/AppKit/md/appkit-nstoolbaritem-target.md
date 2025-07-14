

- AppKit
- NSToolbarItem
-  target 

Instance Property

# target

The object that defines the action method the toolbar item calls when clicked.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS

``` source
@MainActor
weak var target: AnyObject? { get set }
```

## Discussion

If you set this property to `nil`, the toolbar item attempts to execute its action method on the first responder. If the first responder doesn’t implement the action method, it forwards the request up the responder chain.

If you assign a custom view to the toolbar item, modifying this property updates the `target` property of the view, if one exists. If the item doesn’t contain a custom view, the toolbar item manages the target object directly.

## See Also

### Performing the item’s action

var action: Selector?

The action method to call when someone clicks on the toolbar item.

