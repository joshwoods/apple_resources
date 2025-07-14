

- UIKit
- UIBarButtonItem
-  init(systemItem:primaryAction:menu:) 

Initializer

# init(systemItem:primaryAction:menu:)

Creates an item using the specified system item, primary action, and context menu.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
@MainActor @preconcurrency
convenience init(
    systemItem: UIBarButtonItem.SystemItem,
    primaryAction: UIAction? = nil,
    menu: UIMenu? = nil
)
```

## Parameters 

`systemItem`  

The system item to use as the first item on the bar. For possible values, see UIBarButtonItem.SystemItem.

`primaryAction`  

A UIAction to associate with the item. The system item doesn’t use the action to configure its title and image.

`menu`  

The menu to present. The context menu displays in response to a person tapping the item.

## Return Value

A newly initialized UIBarButtonItem.

## See Also

### Creating system items

convenience init(barButtonSystemItem: UIBarButtonItem.SystemItem, target: Any?, action: Selector?)

Creates an item using the specified system item, target, and action.

enum SystemItem

Constants that define system-supplied images for bar button items.

