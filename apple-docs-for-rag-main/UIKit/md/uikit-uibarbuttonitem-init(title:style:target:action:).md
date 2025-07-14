

- UIKit
- UIBarButtonItem
-  init(title:style:target:action:) 

Initializer

# init(title:style:target:action:)

Creates an item using the specified title, style, target, and action.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
convenience init(
    title: String?,
    style: UIBarButtonItem.Style,
    target: Any?,
    action: Selector?
)
```

## Parameters 

`title`  

The item’s title. If `nil`, a title doesn’t appear.

`style`  

The style of the item. For possible values, see UIBarButtonItem.Style.

`target`  

The object that receives the `action` message.

`action`  

The action to send to `target` when a person selects this item.

## Return Value

A newly initialized UIBarButtonItem.

## See Also

### Related Documentation

convenience init(barButtonSystemItem: UIBarButtonItem.SystemItem, target: Any?, action: Selector?)

Creates an item using the specified system item, target, and action.

### Creating items of a specific style

convenience init(image: UIImage?, style: UIBarButtonItem.Style, target: Any?, action: Selector?)

Creates an item using the specified image, style, target, and action.

convenience init(image: UIImage?, landscapeImagePhone: UIImage?, style: UIBarButtonItem.Style, target: Any?, action: Selector?)

Creates an item using the specified images, style, target, and action.

