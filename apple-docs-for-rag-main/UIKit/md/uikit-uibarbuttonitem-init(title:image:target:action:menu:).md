

- UIKit
- UIBarButtonItem
-  init(title:image:target:action:menu:) 

Initializer

# init(title:image:target:action:menu:)

Creates a plain-style item using the specified title, image, target, action, and context menu.

iOS 16.0+iPadOS 16.0+Mac CatalysttvOS 16.0+visionOS

``` source
@MainActor @preconcurrency
convenience init(
    title: String?,
    image: UIImage?,
    target: AnyObject?,
    action: Selector?,
    menu: UIMenu? = nil
)
```

## Parameters 

`title`  

The item’s title. If `nil`, a title doesn’t appear.

`image`  

The item’s image. If `nil`, an image doesn’t appear.

The images displayed on the bar derive from this image. If this image is too large to fit on the bar, it’s scaled to fit. Typically, the size of a toolbar and navigation bar image is `20` x `20` points. The system uses the alpha values in the source image to create the images, ignoring opaque values.

`target`  

The object that receives the `action` message.

`action`  

The action to send to `target` when a person selects this item.

`menu`  

The menu to present. The context menu displays in response to a person tapping the item.

## Return Value

A newly initialized UIBarButtonItem.

## See Also

### Creating items

convenience init(title: String?, image: UIImage?, primaryAction: UIAction?, menu: UIMenu?)

Creates a plain-style item using the specified title, image, primary action, and context menu.

init()

Initializes the item to its default state.

init?(coder: NSCoder)

Creates an item from data in an unarchiver.

