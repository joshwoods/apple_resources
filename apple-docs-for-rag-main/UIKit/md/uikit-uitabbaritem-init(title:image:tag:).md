

- UIKit
- UITabBarItem
-  init(title:image:tag:) 

Initializer

# init(title:image:tag:)

Creates a tab bar item that displays a title and an image.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
convenience init(
    title: String?,
    image: UIImage?,
    tag: Int
)
```

## Parameters 

`title`  

The item’s title.

`image`  

The item’s source image.

`tag`  

An integer you use to identify the object.

## Discussion

Use `nil` for `title` or `image` to not display that element.

By default, the item displays the same image regardless of its selected state. To display a different image for the selected state, set its selectedImage property. The item creates the images it displays from the alpha values in the source images. To prevent system tinting, use images with the UIImage.RenderingMode.alwaysOriginal rendering mode. The item clips any image that’s larger than its bounds.

## See Also

### Creating a tab bar item

convenience init(tabBarSystemItem: UITabBarItem.SystemItem, tag: Int)

Creates a tab bar item using a system-provided configuration.

convenience init(title: String?, image: UIImage?, selectedImage: UIImage?)

Creates a tab bar item that toggles the image it displays when its selected state changes.

init()

Creates a tab bar item with a default configuration.

init?(coder: NSCoder)

Creates a tab bar item from a serialized instance.

enum SystemItem

Constants that represent the system tab bar items.

