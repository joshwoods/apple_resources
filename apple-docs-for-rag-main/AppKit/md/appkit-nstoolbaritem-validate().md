

- AppKit
- NSToolbarItem
-  validate() 

Instance Method

# validate()

Validates the toolbar item’s menu and its ability to perfrom its action.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS

``` source
@MainActor
func validate()
```

## Discussion

Typically, you don’t call this method directly. When automatic validation is enabled, the toolbar calls this method to validate the item. For standard toolbar items — that is, items without a custom view — the validation process checks whether the item can perform its associated action successfully and enables or disables the item accordingly. The process also validates the associated menu item. When someone switches to another app or window, the automatic validation process disables the item automatically.

If the toolbar item has a custom view, subclass NSToolbarItem and override this method to perform the validation yourself. After you validate your custom toolbar item, update the isEnabled property. You don’t need to call `super` in your implementation.

If you disable automatic validation, toolbar items remain enabled and clickable, including when someone switches to another app or window. However, you can still call this method manually to validate the toolbar item.

## See Also

### Related Documentation

var isEnabled: Bool

A Boolean value that indicates whether the item is enabled.

### Validating the item

var autovalidates: Bool

A Boolean value that indicates whether the toolbar automatically validates the item.

