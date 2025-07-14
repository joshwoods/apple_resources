

- UIKit
- UITabBarItem
-  init() 

Initializer

# init()

Creates a tab bar item with a default configuration.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
init()
```

## See Also

### Creating a tab bar item

convenience init(tabBarSystemItem: UITabBarItem.SystemItem, tag: Int)

Creates a tab bar item using a system-provided configuration.

convenience init(title: String?, image: UIImage?, tag: Int)

Creates a tab bar item that displays a title and an image.

convenience init(title: String?, image: UIImage?, selectedImage: UIImage?)

Creates a tab bar item that toggles the image it displays when its selected state changes.

init?(coder: NSCoder)

Creates a tab bar item from a serialized instance.

enum SystemItem

Constants that represent the system tab bar items.

