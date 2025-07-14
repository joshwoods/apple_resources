

- UIKit
- UIBarButtonItem
-  init(image:landscapeImagePhone:style:target:action:) 

Initializer

# init(image:landscapeImagePhone:style:target:action:)

Creates an item using the specified images, style, target, and action.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
convenience init(
    image: UIImage?,
    landscapeImagePhone: UIImage?,
    style: UIBarButtonItem.Style,
    target: Any?,
    action: Selector?
)
```

## Parameters 

`image`  

The item’s image. If `nil`, an image doesn’t appear.

`landscapeImagePhone`  

The image to use for the item in landscape bars in the UIUserInterfaceIdiom.phone idiom.

`style`  

The style of the item. For possible values, see UIBarButtonItem.Style.

`target`  

The object that receives the `action` message.

`action`  

The action to send to `target` when a person selects this item.

## Return Value

A newly initialized UIBarButtonItem.

## See Also

### Creating items of a specific style

convenience init(title: String?, style: UIBarButtonItem.Style, target: Any?, action: Selector?)

Creates an item using the specified title, style, target, and action.

convenience init(image: UIImage?, style: UIBarButtonItem.Style, target: Any?, action: Selector?)

Creates an item using the specified image, style, target, and action.

