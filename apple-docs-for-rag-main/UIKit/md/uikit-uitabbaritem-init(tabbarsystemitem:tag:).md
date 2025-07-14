

- UIKit
- UITabBarItem
-  init(tabBarSystemItem:tag:) 

Initializer

# init(tabBarSystemItem:tag:)

Creates a tab bar item using a system-provided configuration.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
convenience init(
    tabBarSystemItem systemItem: UITabBarItem.SystemItem,
    tag: Int
)
```

## Parameters 

`systemItem`  

The preferred system item. For possible values, see UITabBarItem.SystemItem.

`tag`  

An integer you use to identify the object.

## Discussion

You can’t change the title and image properties of an item this method creates.

## See Also

### Creating a tab bar item

convenience init(title: String?, image: UIImage?, tag: Int)

Creates a tab bar item that displays a title and an image.

convenience init(title: String?, image: UIImage?, selectedImage: UIImage?)

Creates a tab bar item that toggles the image it displays when its selected state changes.

init()

Creates a tab bar item with a default configuration.

init?(coder: NSCoder)

Creates a tab bar item from a serialized instance.

enum SystemItem

Constants that represent the system tab bar items.

