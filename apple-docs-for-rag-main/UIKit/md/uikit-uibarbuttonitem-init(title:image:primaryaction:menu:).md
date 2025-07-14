

- UIKit
- UIBarButtonItem
-  init(title:image:primaryAction:menu:) 

Initializer

# init(title:image:primaryAction:menu:)

Creates a plain-style item using the specified title, image, primary action, and context menu.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
@MainActor @preconcurrency
convenience init(
    title: String? = nil,
    image: UIImage? = nil,
    primaryAction: UIAction? = nil,
    menu: UIMenu? = nil
)
```

## Parameters 

`title`  

The item’s title.

`image`  

The item’s image.

The images displayed on the bar derive from this image. If this image is too large to fit on the bar, it’s scaled to fit. Typically, the size of a toolbar and navigation bar image is `20` x `20` points. The system uses the alpha values in the source image to create the images, ignoring opaque values.

`primaryAction`  

A UIAction to associate with the item, which the item uses to configure its title and image. If you specify `primaryAction`, it takes precedence over `title` and `image`.

`menu`  

The menu to present. The context menu displays in response to a person tapping the item.

## Return Value

A newly initialized UIBarButtonItem.

## See Also

### Creating items

convenience init(title: String?, image: UIImage?, target: AnyObject?, action: Selector?, menu: UIMenu?)

Creates a plain-style item using the specified title, image, target, action, and context menu.

init()

Initializes the item to its default state.

init?(coder: NSCoder)

Creates an item from data in an unarchiver.

