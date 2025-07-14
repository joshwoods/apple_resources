

- AppKit
- NSToolbarItem
-  action 

Instance Property

# action

The action method to call when someone clicks on the toolbar item.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS

``` source
@MainActor
var action: Selector? { get set }
```

## Discussion

If you assign a custom view to the toolbar item, modifying this property updates the `action` property of the view or calls the `setAction:` method, if one of them exists. If the item doesn’t contain a custom view, the toolbar item manages the action directly.

## See Also

### Performing the item’s action

var target: AnyObject?

The object that defines the action method the toolbar item calls when clicked.

