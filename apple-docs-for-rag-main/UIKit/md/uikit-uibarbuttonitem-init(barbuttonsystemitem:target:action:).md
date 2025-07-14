

- UIKit
- UIBarButtonItem
-  init(barButtonSystemItem:target:action:) 

Initializer

# init(barButtonSystemItem:target:action:)

Creates an item using the specified system item, target, and action.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
convenience init(
    barButtonSystemItem systemItem: UIBarButtonItem.SystemItem,
    target: Any?,
    action: Selector?
)
```

## Parameters 

`systemItem`  

The system item to use as the first item on the bar. For possible values, see UIBarButtonItem.SystemItem.

`target`  

The object that receives the `action` message.

`action`  

The action to send to `target` when a person selects this item.

## Return Value

A newly initialized UIBarButtonItem.

## See Also

### Related Documentation

convenience init(image: UIImage?, style: UIBarButtonItem.Style, target: Any?, action: Selector?)

Creates an item using the specified image, style, target, and action.

convenience init(title: String?, style: UIBarButtonItem.Style, target: Any?, action: Selector?)

Creates an item using the specified title, style, target, and action.

### Creating system items

convenience init(systemItem: UIBarButtonItem.SystemItem, primaryAction: UIAction?, menu: UIMenu?)

Creates an item using the specified system item, primary action, and context menu.

enum SystemItem

Constants that define system-supplied images for bar button items.

