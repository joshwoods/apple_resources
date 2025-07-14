

- UIKit
- UITabBarItem
-  init(title:image:selectedImage:) 

Initializer

# init(title:image:selectedImage:)

Creates a tab bar item that toggles the image it displays when its selected state changes.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
convenience init(
    title: String?,
    image: UIImage?,
    selectedImage: UIImage?
)
```

## Parameters 

`title`  

The item’s title.

`image`  

The item’s source image.

`selectedImage`  

The source image the item uses when the user selects it.

## Discussion

Use `nil` for `title` or `image` if you don’t want to display that element.

If you don’t provide `selectedImage`, the item uses `image` for both selection states. The item creates the images it displays from the alpha values in the source images. To prevent system tinting, use images with the UIImage.RenderingMode.alwaysOriginal rendering mode. The item clips any image that’s larger than its bounds.

## See Also

### Creating a tab bar item

convenience init(tabBarSystemItem: UITabBarItem.SystemItem, tag: Int)

Creates a tab bar item using a system-provided configuration.

convenience init(title: String?, image: UIImage?, tag: Int)

Creates a tab bar item that displays a title and an image.

init()

Creates a tab bar item with a default configuration.

init?(coder: NSCoder)

Creates a tab bar item from a serialized instance.

enum SystemItem

Constants that represent the system tab bar items.

