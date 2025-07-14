

- AppKit
- NSToolbarItem
-  autovalidates 

Instance Property

# autovalidates

A Boolean value that indicates whether the toolbar automatically validates the item.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS

``` source
@MainActor
var autovalidates: Bool { get set }
```

## Discussion

If the value of this property is true, the toolbar automatically validates the item; otherwise, it doesn’t validate the item automatically. The default value of this property is true.

## See Also

### Validating the item

func validate()

Validates the toolbar item’s menu and its ability to perfrom its action.

